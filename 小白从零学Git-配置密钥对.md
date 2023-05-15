要生成用于连接 GitHub 的 SSH 密钥对，可以按照以下步骤操作：

1. 打开终端或命令提示符窗口。

2. 输入以下命令：

   ```
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```

   其中，`your_email@example.com` 是您在 GitHub 帐户中使用的电子邮件地址。

3. 按 Enter 键确认将密钥保存在默认位置（一般为 `~/.ssh/id_rsa`）。

4. 输入一个密码，以保护您的私钥。如果您不想设置密码，可以直接按 Enter 键跳过此步骤。

5. 生成密钥对后，将会显示公钥和私钥的路径。公钥的路径是默认路径，即 `~/.ssh/id_rsa.pub`。您需要将公钥添加到您的 GitHub 帐户中。

6. 登录到您的 GitHub 帐户，并转到“Settings”（设置）> “SSH and GPG keys”（SSH 和 GPG 密钥）> “New SSH Key”（新 SSH 密钥）。

7. 在“Key”字段中，将您的公钥复制并粘贴到其中。

8. 提交新密钥后，您可以使用 `ssh -T git@github.com` 命令来测试您的 SSH 连接是否成功。如果您看到“Hi username! You've successfully authenticated, but GitHub does not provide shell access.”（您已成功进行身份验证，但 GitHub 不提供 shell 访问权限）的消息，则表示您已成功连接到 GitHub。

这样，您就成功生成了一个用于连接 GitHub 的 SSH 密钥对，并将公钥添加到您的 GitHub 帐户中。
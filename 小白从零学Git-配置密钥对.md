Ҫ������������ GitHub �� SSH ��Կ�ԣ����԰������²��������

1. ���ն˻�������ʾ�����ڡ�

2. �����������

   ```
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```

   ���У�`your_email@example.com` ������ GitHub �ʻ���ʹ�õĵ����ʼ���ַ��

3. �� Enter ��ȷ�Ͻ���Կ������Ĭ��λ�ã�һ��Ϊ `~/.ssh/id_rsa`����

4. ����һ�����룬�Ա�������˽Կ������������������룬����ֱ�Ӱ� Enter �������˲��衣

5. ������Կ�Ժ󣬽�����ʾ��Կ��˽Կ��·������Կ��·����Ĭ��·������ `~/.ssh/id_rsa.pub`������Ҫ����Կ��ӵ����� GitHub �ʻ��С�

6. ��¼������ GitHub �ʻ�����ת����Settings�������ã�> ��SSH and GPG keys����SSH �� GPG ��Կ��> ��New SSH Key������ SSH ��Կ����

7. �ڡ�Key���ֶ��У������Ĺ�Կ���Ʋ�ճ�������С�

8. �ύ����Կ��������ʹ�� `ssh -T git@github.com` �������������� SSH �����Ƿ�ɹ��������������Hi username! You've successfully authenticated, but GitHub does not provide shell access.�������ѳɹ����������֤���� GitHub ���ṩ shell ����Ȩ�ޣ�����Ϣ�����ʾ���ѳɹ����ӵ� GitHub��

���������ͳɹ�������һ���������� GitHub �� SSH ��Կ�ԣ�������Կ��ӵ����� GitHub �ʻ��С�
һ��
1.������linux�²鿴~Ŀ¼�����Ƿ���.ssh�ļ��У���û�����shell���롰ssh-keygen -t rsa -C "exmaple@mail.com"������SSH Key;������windows�´�git bash�������������ssh key��
2.�����ú󣬵�½github�˺ţ���setting�����ҵ�ssh keys���ssh key���������⣬key����.ss�ļ���id_sra.pub���������,a���
3.����ͬ���Ĳ������1,2
4.д�����ļ�config:
# salvete                                                        
Host github.com 
HostName github.com
User git
IdentityFile ~/.ssh/id_rsa
# salveter                                                                           
Host salveter
HostName github.com
User git
IdentityFile ~/.ssh/salveter/id_rsa
5.�����Ƿ�������У�
�ֱ�����
ssh -T git@github.com
ssh -T git@salveter
��������¶�����
���˵�һ�����Ѿ����

����
Ψһֵ����Ҫע����ǹ���ʱ��github����git@github.com:salveter/two_or_more_username.git�ǲ��еģ���Ϊgithub.com�Ѿ���salveteռ����,����Ӧ�ý�github.com�滻��salveter,��git@salvete:salveter/two_or_more_username.git
Ȼ��󹦸��

一、
1.若是在linux下查看~目录下面是否有.ssh文件夹，若没有则打开shell输入“ssh-keygen -t rsa -C "exmaple@mail.com"”创建SSH Key;若是在windows下打开git bash输入如上命令创建ssh key。
2.创建好后，登陆github账号，在setting栏中找到ssh keys添加ssh key，标题自拟，key输入.ss文件中id_sra.pub里面的内容,a完成
3.按照同样的步骤完成1,2
4.写配置文件config:
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
5.测试是否可以运行：
分别输入
ssh -T git@github.com
ssh -T git@salveter
正常情况下都可以
至此第一部分已经完成

二、
唯一值得需要注意的是关联时将github输入git@github.com:salveter/two_or_more_username.git是不行的，因为github.com已经被salvete占用了,所以应该将github.com替换成salveter,即git@salvete:salveter/two_or_more_username.git
然后大功告成

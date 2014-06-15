#github 使用

###### 第一章 [配置ssh](https://help.github.com/articles/generating-ssh-keys)

step1. 进入C:\Users\TDP\.ssh目录

step2. 生成ssh key
```
C:\Users\TDP>ssh-keygen -t rsa -C "mapleleaf1988@126.com"
Generating public/private rsa key pair.
Enter file in which to save the key (//.ssh/id_rsa): */c/Users/TDP/.ssh/id_rsa*
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/TDP/.ssh/id_rsa.
Your public key has been saved in /c/Users/TDP/.ssh/id_rsa.pub.
The key fingerprint is:
4a:05:88:e3:0f:be:98:77:a5:4e:87:85:8a:98:42:6c mapleleaf1988@126.com

$clip < ./.ssh/id_rsa.pub
```

step3. 在github中添加ssh key
**注意： ssh key 的title必须是github用户名**






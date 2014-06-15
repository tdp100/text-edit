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


####异常处理
D:\WebstormProjects\text-edit>git push -u gitorigin master
Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

这里是key 没有导入ssh-agent 或者 ssh-agent没有启动，


**[解决办法](https://help.github.com/articles/working-with-ssh-key-passphrases)：**
1. 创建`~/.profile` or `~/.bashrc file`
2. 重启bash ，输入passwrd
3. 重新测试一下: ssh -T tdp100@github.com



#[sublime text 3](http://docs.sublimetext.tw/)


###### 第一章、工具选择
+ 1、文本编辑工具 sublime text 3
+ 2、编辑语法 vim
  + 配置
    `preferences->seting user`
    输入如下python语句
    ```python
    {
		"ignored_packages": [],
		"vintage_start_in_command_mode": true,
		"vintage_ctrl_keys": true
	}
	```
+ 3、vim 命令与编辑状态切换快捷键 `esc` or `ctrl+[`
+ 4、vim 常见的快捷键
	+ 1. 缩进  `ctrl + [`  or `ctrl + ]`
+ 5、sublime 常见的快捷键
    + 1. goto anywhere　`ctrl + p`
    + 2. 文件内模糊搜索 `ctrl + p #` or `ctrl + ;`
    + 3. 搜索文件内的symbols `ctrl + p @` or `ctrl + r`
    + 4. 跳转到文件内的某一行 `ctrl + p :` or `ctrl + g`


###### 第二章、编辑
+ 1、多重选择
	+ 1. 重复选择单词
		1. 选择word `ctrl + d`
		2. 重复`ctrl + d`可以选择更多该word
		3. 如果想跳过其中的一个,使用 `ctrl + k + d`
	+ 2.竖直多选, `ctrl + alt + 方向键`
+ 2、恢复操作 `ctrl + u`
+ 3、合并多行 `ctrl + j`
+ 4、转换大小写
    + 1. 转换为大写 `ctrl + k + u`
    + 2. 转换为小写 `ctrl + k + l`
    + 3. 首字母转换, 自定义快捷键 `ctrl + k + t`
	     `json [ { "keys": ["ctrl+k", "ctrl+t"], "command": "title_case" } ]`

###### 第三章、搜索
+ 1、文件内搜索 `ctrl + f`
    + 查找下一个 `enter`
    + 查找上一个 `shift + enter`
    + 全选 `alt + enter`
    + perl 正则表达式式搜索 `alt + r`
    + 区分大小写搜索 `alt + c`
    + 完全匹配 `alt + w`
+ 2、搜索范围 `ctrl + shif + f`
    + where 中使用 unix-style的路径表示法，例如：`../path/to/directories`，也可以是绝对路径
    + 排除特定的文件或目录，例如：-*.txt 或 -/path/to/ignore/*;
    + 只搜索已经打开的目录或者文件：<open files>、<open files>；
    + 不同的条件可以用逗号（,）隔开

###### 第四章、[包管理](http://docs.sublimetext.info/en/latest/extensibility/plugins.html)
+ 1、由于sublime text 3 不自带package controller 包,所以需要使用 [Will Bond](http://wbond.net/)开发的plugin, [安装指南](https://sublime.wbond.net/installation#st3)
     `The simplest method of installation is through the Sublime Text console. The console is accessed via the ctrl+` shortcut or the View > Show Console menu. Once open, paste the appropriate Python code for your version of Sublime Text into the console.`
     ```python
     import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
     ```
+ 2、 安装包 `ctrl + shift + p`  然后输入 `install package`

+ 3、安装terminal plugin， 快速打开控制台
     + 1. install terminal
     + 2. 默认快捷键　`ctrl + shift + t`
     + 3. 修改快捷键为 `alt + f12` 与 webstorm保持一致
     
    
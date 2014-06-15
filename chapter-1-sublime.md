#sublime text 3

*************************
积少成大，熟练使用工具，提升工作效率

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

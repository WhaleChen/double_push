# 简介
一个简单的python脚本，用于实现对GitHub和Gitbook下的双推。

# 下载
点击右下角的`Clone in Desktop`或者`Download Zip`将代码下载到本地。
或者使用命令行命令
```
git clone https://github.com/wp-lai/double_push.git
```

# 使用
将`double_push.py`移动到使用git的文件夹里。然后在命令行里执行
```
python double_push.py {user_name} {github_repo_name} {gitbook_repo_name}
```
里面包含三个参数
+ 参数1是GitHub和Gitbook上的用户名
+ 参数2是GitHub上代码库的名称
+ 参数3是Gitbook上书籍的名称

例如，用户名是wp-lai，GitHub上代码库名称为my_omooc2，Gitbook上书籍名称为learn-python，而在个人电脑中内容存在OMOOC2py文件夹下。

则将`double_push.py`移动到OMOOC2py文件夹根目录下。
然后在命令行里执行
```
python double_push.py wp-lai my_omooc2 learn-python
```

命令执行成功会显示`Mission Complete`

这之后，本地代码库进行修改并完成commit之后
执行'git push'，就可以同时push给GitHub和Gitbook

# 注意事项
1. 确认在GitHub和Gitbook里已经建立了相应的代码库，若没有的话，新建一个即可。

2. 脚本命令执行时，shell的当前工作文件夹需是代码文件夹。Mac下用`pwd`可以显示shell的当前目录，如果不是代码文件夹，则用`cd`命令更改shell的当前文件夹。



# 改进和建议
欢迎大家在issue中指出代码问题和提出修改建议，也希望大家fork以及提交pull request。

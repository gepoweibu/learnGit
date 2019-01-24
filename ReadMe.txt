IDEA git设置和使用：
1.file-->setting-->version contronl-->Git-->Path to Gitexecutable-->设置git.exe 文件路径
2.VCS-->Enable Version Contronl integration
3.git-->add-->commit-->push
4.Intellij IDEA中Git本地仓库必须建立在当前项目文件夹下，其它自定义的位置不支持；(曾陷入此坑无法自拔)
5.version control -->alt+9
6.IDEA Terminal 调用 bash.exe 数据Unicode编码问题解决：
找到git安装目录下的etc/bash.bashrc文件，在文件末尾添加-->
export LANG="zh_CN.UTF-8"
export LC_ALL="zh_CN.UTF-8"
7.git 编码设置：
$ git config --global core.quotepath false   显示 status 编/git内部编码转换设置

$ git config --global gui.encoding utf-8  GUI界面编码

$ git config --global i18n.commit.encoding utf-8  提交信息编码

$ git config --global i18n.logoutputencoding utf-8  输出log编码

$ export LESSCHARSET=utf-8 Linux系统需要设置
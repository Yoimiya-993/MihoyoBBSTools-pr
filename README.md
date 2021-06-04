# 自动米游社

使用Python3编写的米游社项目

## 如何使用

Windows：

打开[python官网](https://www.python.org/downloads/)，点击Download下载最新版Python并进行安装

打开[Git官网](https://git-scm.com/)，点击`Download x.xx.1x for Windows`下载git并进行安装

找到一个合适的位置，用`Shift+右键`打开你的命令提示符(cmd)/powershell，然后粘贴以下内容`git clone https://github.com/Womsxd/AutoMihoyoBBS.git && cd AutoMihoyoBBS && pip install -r requirements.txt && explorer .\config`

接着，在弹出的文件管理器的窗口这里复制，`config.json.example`并改名为`config.json`，如果需要使用多用户的功能的话请改名成`xxx.json`，
请使用vscode/notepad++等文本编辑器打开`config.json`，使用[获取Cookie](#获取米游社的Cookie)里面的方法来获取Cookie，在成功获取Cookie后粘贴到`"mihoyobbs_Cookies": "`的后面，之后回到你的命令提示符(cmd)/powershell，输入`python main.py`来进行执行，多用户的请使用`python main_multi.py`，多用户在需要自动执行的情况下请使用`python main_multi.py autorun`

## 获取米游社的Cookie

1、打开你的浏览器，进入无痕/隐身模式

2、打开`http://bbs.mihoyo.com/ys/`并进行登入操作

3、按下键盘上的`F12`或右键检查，打开开发者工具

4、点击Console

5、复制`var cookie=document.cookie;var ask=confirm('Cookie:'+cookie+'\n\nDo you want to copy the cookie to the clipboard?');if(ask==true){copy(cookie);msg=cookie}else{msg='Cancel'}`，在Console这里进行粘贴后按回车执行，并在确认无误后点击确定。

6、Cookie已经复制到你的粘贴板上了

## ToDo

~~1、多用户支持~~已经支持

## 注意小范围使用，请勿大范围传播这个项目，懂得都懂

废话（

## Q&A

Q：这个项目是干什么的？

A：这是一个米游社的自动签到项目，包含了米游币和原神

Q：为什么要写这个项目？

A：对github上现在的几个项目感觉可以配置的的地方比较少，于是就写了这个项目

## 项目更新

请使用`git clone`克隆本项目，更新清使用`git pull`，应为会合并commits的关系，如果遇到无法更新请使用`git reset --hard HEAD && git pull -r`强制pull最新源码，如果还是无法更新请备份config文件夹后重新克隆本项目。

## 本项目参考了以下项目

[XiaoMiku01/miyoubiAuto](https://github.com/XiaoMiku01/miyoubiAuto)

## License

[MIT License](https://github.com/Womsxd/AutoMihoyoBBS/blob/master/LICENSE)

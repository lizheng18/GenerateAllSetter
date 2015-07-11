﻿
#介绍

GenerateAllSetter 是给intellij idea开发的一个生成调用Set方法的插件，在开发时有时候会遇到初始化domain时需要
调用很多Set方法，需要人工一个一个操作，非常的麻烦，所以开发了这个插件，提高效率

#关于我

从事电商的java码农，目前我在[okhqb.com](http://www.okhqb.com)工作。我的[个人主页](http://www.okhjp.com/)。

#插件安装

1.直接下载GenerateAllSetter.jar放到本地磁盘，
2.然后在intellij idea 插件安装，选install plugin from disk 安装重启即可使用

#插件使用

在new domain时，需要初始化调用所有Set方法时，只需要将光标移动到类上，
然后按快捷键( Ctrl+Shit+G )或(alt+insert -input all set>,就会自动生成代码

#插件开发
参见[intellij idea development](http://confluence.jetbrains.com/display/IDEADEV/Getting+Started+with+Plugin+Development#GettingStartedwithPluginDevelopment-anchor5)

#高版本不能使用问题
1.如果使用jdk1.7以上开发，会出现问题
由于 Idea 默认是使用 JRE 1.6 的，如果要使用 JRE 1.7 可以通过修改文件 /Applications/IntelliJ\ IDEA\ 14\ CE.app/Contents/Info.plist
{code}
<key>JVMVersion</key>
<string>1.6*</string>
{code}
修改为
{code}
<key>JVMVersion</key>
<string>1.7+</string>
{code}

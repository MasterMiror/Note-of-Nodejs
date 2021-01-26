#Nodejs笔记

*Author:Alex

这部分是Node的基础内容,涉及到一些基本的代码.

*CommonJS规范*

在Node中可以一个JS就是一个模块.

在Node中通过require()引入外部模块

通过exports向外暴露变量

引用到当前js需要用require()引入 用var声明一个变量,然后再调用. var package = require('path')大概是这个格式

模块大致可以分成两大类,一类是核心模块(由node引擎提供的模块),另一类是文件模块(用户自己创建的)

核心模块的标识就是自己模块的名字,文件模块的标识是文件的路径(可以是绝对也可以是相对)

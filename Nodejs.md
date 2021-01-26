#Nodejs笔记

*Author:Alex

这部分是Node的基础内容,涉及到一些基本的代码.

*CommonJS规范*

在Node中可以一个JS就是一个模块.

在Node中通过require()引入外部模块

通过exports向外暴露变量

引用到当前js需要用require()引入 用var声明一个变量,然后再调用. var package = require('path')大概是这个格式

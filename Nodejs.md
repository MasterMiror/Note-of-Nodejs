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

*不用var,直接声明则为全局变量*

实际这些js执行的时候都是被包装在一个函数中.

function(exports,require,module,__filename,__dirname){函数体}

exports用来暴露变量或函数

require引入外部模块

module代表当前模块本身

故exports和module.exports效果是一样的

__filename是当前模块的完整路径

__dirname是当前所在文件夹的完整路径

注意exports里的东西和module.export里的东西指向的是同一个,module.exports = {name} 和exports.name指向的是同一个东西.

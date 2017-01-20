# Atom 爱上 JS

<http://haoqicat.com/atom-love-js>

> index.mp4

一个摩登 Nodejs 开发者应该具备编辑器使用技巧大全。

**为谁而写？**

还没有理解什么是开发编辑器的新手，或者是已经使用 Sublime 一段时间，但是想要切换到 Atom 编辑器的老手。

**内容简介**

瞄准 React + Nodejs 开发，内容为 JS 开发者量身打造，务求实用。

## 第一章：宏观先说说

### [为何离开 Sublime Text ？](http://haoqicat.com/atom-love-js/1-why-leave-sublime)

> 1-why-leave-sublime.mp4

**Sublime 的主要问题**
我使用 sublime 编辑器也有比较长的时间了，根据自己的经验我对 sublime 主要不满的地方还是
- sublime text 是收费软件，尽管不购买也可以使用，但经常会弹出购买提示框
- sublime 对中文的支持不好，跟中文输入法的配合常常出现问题
- sublime 里面 `ctrl + e` 不能跳到行尾，这种系统快捷键不兼容，让我很不爽

所以打算换 atom，听说他有这些个有点：

- github 公司开发的，我还是比较迷信大厂，对 git 支持好
- 基于 node js 开发，对node js 支持好
- 中文支持好，跨平台
- 社区活跃
- 兼容 sublime 的大多数快捷键
- 切换过来成本低
- 对 markdown 支持好

### [安装和启动 Atom 的正确姿势](http://haoqicat.com/atom-love-js/2-install)

> 2-install.mp4

- mac 直接在官网下载安装
- 系统命令 `atom .`
- atom 窗口间切换 `ctrl + 闪引号`

### [装包](http://haoqicat.com/atom-love-js/3-package)

> 3-package.mp4

**装包主要有 2 中方式**

- 命令面板中安装、删除、禁用
- 命令行安装 `apm insall theme-name-ui`
- 在包配置页面中可以对包进行详细的设置

## 第二章：通用功能点

### [定制主题](http://haoqicat.com/atom-love-js/4-theme)

> 4-theme.mp4

**安装个性化主题**

- `apm search theme-name`
- `apm install atom-material-ui`
- 命令面板中 `change theme`
- theme 分为 2 种：UI theme 和 Syntax theme

### [命令行](http://haoqicat.com/atom-love-js/5-terminal)

> 5-terminal.mp4

- open 终端：atom-open-terminal-here
- advanced-open-file

### [git](http://haoqicat.com/atom-love-js/6-git)

> 6-git.mp4

未保存到 git 版本中的内容会高亮显示，默认安装了 gitdiff 这个 package

### [快速查找](http://haoqicat.com/atom-love-js/7-find)

> 7-find.mp4

- cmd+p 打开面板，支持模糊查找
- settings -> ignored names 中添加 node_modules 等需要手工忽略的文件
- cmd+f 查找
- shift+cmd+f 全项查找
- 默认已安装 find-and-replace, fuzzy-finder 包，可以自行修改设置

## 第三章：自动补齐

### [默认补齐行为](http://haoqicat.com/atom-love-js/8-default)

> 8-default.mp4

- buffer 当前已有字符串
- 预装的 snippet 可以到命令面板 snippet available 查看
- settings -> packages -> language-javascript snippet 查看 javascript 的可用 snippet

### [创建自己的 snippets](http://haoqicat.com/atom-love-js/9-snippet)

> 9-snippet.mp4

**创建自己的 snippet**

- 命令面板中 -> open your snippet，创建一个叫 snippets.cson 的文件
- snip+ Tab 自动补齐一个 snippet 骨架
- 在当前文件中 alt+cmd+p 得到当前文件类型的类型文件写法

### [Emmet](http://haoqicat.com/atom-love-js/10-emmet)

> 10-emmet.mp4

- `apm install emmet`, 安装以后需要重启 atom 才可以生效
- ctrl+w 添加一个包裹的父元素
- 把光标停留在标签上，然后 cmd+单引号 删除一层标签
- settings -> packages -> emmet 查看更多配置项

## 第四章：框架自定制

### [Nodejs](http://haoqicat.com/atom-love-js/11-nodejs)

可以自定义 node.js 常用的 snippets

推荐一个 package：[atom-ternjs](https://github.com/tststs/atom-ternjs)


> 11-nodejs.mp4

### [React](http://haoqicat.com/atom-love-js/12-react)

> 12-react.mp4

- [atom-react 包](https://github.com/orktes/atom-react)
- <https://nuclide.io/> 这个项目值得关注

## 第五章：总结

### [常用快捷键](http://haoqicat.com/atom-love-js/13-shortcuts)

> 13-shortcuts.mp4

**行操作**

- shift+ctrl+k 删除当前行
- cmd+j 合并下一行
- ctrl+cmd+箭头 移动当前行
- cmd+l 选中当前行，重复可选中多行

**多点编辑**

- cmd+click 多个光标
- cmd+shift+l 选中多行并可编辑
- cmd+d 选中和当前字符串相同的字符串，并可编辑

**页面操作**

- shift+cmd+t 回复刚刚关闭的页面

**窗格操作**

- cmd+k 打开新窗格
- cmd+\ 关闭目录树

更多快捷键，参考：<http://flight-manual.atom.io/using-atom/sections/atom-selections/>

查看全部快捷键，命令面板 key binds

*The End*

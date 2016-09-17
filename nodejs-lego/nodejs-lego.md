# [Nodejs 乐高](http://haoqicat.com/nodejs-lego)

> 一个全栈摩登 JS 开发者的必备 nodejs 基础

为谁而写？

正在使用 React/Meteor/Express 这些框架进行开发的朋友们。初学 Nodejs 开发的小白，以及开发 Nodejs 一段时间，但是其实希望更深入的了解一下 Nodejs 的一些底层机制的老手。

内容简介

理解何谓非阻塞，异步 IO ，模块化编程，HTTP 服务器这些 Nodejs 的基础知识。另外，每天安装 NPM 包是我们最重要的事情了，所以课程中会自己手动制作发布一个 npm 包，加深我们对 npm 工作方式的理解

## 第一章 Nodejs 生态

### 什么是 nodejs 模块

nodejs 是什么

- Javascript 运行环境
- [npm](https://www.npmjs.com) (Node Package manager)

nodejs 怎么学？

- 后端 [express 框架](http://expressjs.com)
- 前端 [react 框架](http://reactjs.com)
- [ES6 教程](http://es6.ruanyifeng.com)

### [安装 nodejs](http://haoqicat.com/nodejs-lego/1-2-nodejs-install)

- nvm (Node Version Manager)
- cnpm：npm 的淘宝镜像

## 第二章 模块化开发 JS

### [nodejs 模块](http://haoqicat.com/nodejs-lego/2-1-modules)

- require
- module.exports

参考文章：

- <https://liuzhichao.com/p/1669.html>
- <http://www.cnblogs.com/snandy/archive/2012/03/03/2378101.html>

### [內建模块](http://haoqicat.com/nodejs-lego/2-2-built-in-modules)

- `require('fs')`
- `fs.readFile`

## 第三章 异步 IO 和事件

### [异步 IO](http://haoqicat.com/nodejs-lego/3-1-async-io)

- readFile: 异步，完成后执行回调函数
- readFileSync：同步，等待返回结果

参考文章：
- <https://cnodejs.org/topic/4f50dd9798766f5a610b808a>

### [简单的 HTTP 服务器](http://haoqicat.com/nodejs-lego/3-2-http-server)

示例：自己动手写一个 http server

### [事件响应](http://haoqicat.com/nodejs-lego/3-3-event-handling)

- `server.on('connection', function....)`

## 第四章 NPM 实用技巧

### [NPM 简介](http://haoqicat.com/nodejs-lego/4-1-npm-intro)

### [以 express 安装为例](http://haoqicat.com/nodejs-lego/4-2-express)


## 第五章 自己动手做一个 NPM 包

### [发布一个包](http://haoqicat.com/nodejs-lego/5-1-publish)

发布到包到 npm 平台主要涉及的命令

- npm login
- npm whoami
- npm publish

### [使用和升级包](http://haoqicat.com/nodejs-lego/5-2-update)

升级包主要涉及的命令：

- npm publish
- npm install
- npm update package_name

### [依赖](http://haoqicat.com/nodejs-lego/5-3-dependencies)

### [系统命令](http://haoqicat.com/nodejs-lego/5-4-cli)

## 第六章 Goodbye

### [npm 脚本](http://haoqicat.com/nodejs-lego/6-1-npm-scripts)

执行npm-scripts： 

- `npm run-script hello`
- `npm start`

参考文章：

- <https://css-tricks.com/why-npm-scripts/>
- <http://billie66.github.io/TLCL/book/zh/>

### [更多学习资源](http://haoqicat.com/nodejs-lego/6-2-more)

参考资料：

- <https://docs.npmjs.com>
- <http://expressjs.com/>



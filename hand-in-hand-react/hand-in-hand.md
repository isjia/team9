# React 手牵手

**为谁而写？**

注意这并不是一套初级课程。课程是为有 Nodejs + React 基础的同学准备的。作为预备知识，可以先看好奇猫上的 《 React-Express 极简 API 》课程。

**内容简介**

学习 React + Express 前后端分离的架构，MongoDB 使用，JWT 认证方式，权限管理，图片上传，文章增删改查日常操作。

## 第一章：搭建后端开发环境

### [新建一个简单的 Express 应用](http://haoqicat.com/hand-in-hand-react/1-express-env)

> 1-express-env.mp4

创建 `hand-in-hand-demo` 项目@github

### [Express 应用开发必备神器 Nodemon](http://haoqicat.com/hand-in-hand-react/2-nodemon)

> 2-nodemon.mp4

全局安装 `npm install -g nodemon`
启动 `nodemon index.js`

### [MongoDB 数据库入门](http://haoqicat.com/hand-in-hand-react/3-mongo)

> 3-mongo.mp4

### [MongoDB 图形化管理工具](http://haoqicat.com/hand-in-hand-react/4-mongo-express)

> 4-mongo-express.mp4

**Mongo Express**

### [Mongoose 连接两座孤岛之间的桥梁](http://haoqicat.com/hand-in-hand-react/5-mongoose)

> 5-mongoose.mp4

## 第二章：后端实现用户认证接口

### [借助 Mongoose 保存用户信息到 MongoDB 数据库](http://haoqicat.com/hand-in-hand-react/6-user-model)

> 6-user-model.mp4

### [安全的把用户密码保存到数据库](http://haoqicat.com/hand-in-hand-react/7-bcrypt)

> 7-bcrypt.mp4

### [用户认证方式对比](http://haoqicat.com/hand-in-hand-react/8-traditional-auth)

> 8-traditional-auth.mp4

### [JWT 知识科普](http://haoqicat.com/hand-in-hand-react/9-jwt)

> 9-jwt.mp4

JSON Web Token

header.payload.signature

### [调试 API 功能](http://haoqicat.com/hand-in-hand-react/10-debug-api)

> 10-debug-api.mp4

### [实现用户认证接口](http://haoqicat.com/hand-in-hand-react/11-auth-api)

> 11-auth-api.mp4

### [实现基于 JWT 的用户认证接口](http://haoqicat.com/hand-in-hand-react/12-jwt)

> 12-jwt.mp4

## 第三章：搭建前端开发环境

### [搭建前端开发环境](http://haoqicat.com/hand-in-hand-react/13-client-env)

> 13-client-env.mp4

### [引入 Material-UI 组件库美化页面](http://haoqicat.com/hand-in-hand-react/14-mui)

> 14-mui.mp4

### [借助 Radium 工具集，编写导航栏的样式](http://haoqicat.com/hand-in-hand-react/15-nav-bar)

> 15-nav-bar.mp4

### [添加前端路由模块](http://haoqicat.com/hand-in-hand-react/16-react-router)

> 16-react-router.mp4

## 第四章：前端用户登录功能实现

### [编写用户登录表单](http://haoqicat.com/hand-in-hand-react/17-login-form)

> 17-login-form.mp4

### [使用 axios 请求后端用户认证接口](http://haoqicat.com/hand-in-hand-react/18-submit-login-form)

> 18-submit-login-form.mp4

## 第五章：Redux 大显神通

### [创建 Redux Store 传递给 React 组件](http://haoqicat.com/hand-in-hand-react/19-redux-store)

> 19-redux-store.mp4

### [创建与用户认证相关的 Redux Reducer](http://haoqicat.com/hand-in-hand-react/20-redux-reducer)

> 20-redux-reducer.mp4

### [借助 Redux Thunk 实现异步 Action Creator](http://haoqicat.com/hand-in-hand-react/21-redux-action)

> 21-redux-action.mp4

### [React 组件连接 React Store 分发 Redux Action](http://haoqicat.com/hand-in-hand-react/22-react-redux)

> 22-react-redux.mp4

### [前端导航栏体现用户登录状态](http://haoqicat.com/hand-in-hand-react/23-header-state)

> 23-header-state.mp4

### [前端实现用户退出登录功能](http://haoqicat.com/hand-in-hand-react/24-logout)

> 24-logout.mp4

## 第六章：用户注册功能实现

### [后端编写用户注册接口](http://haoqicat.com/hand-in-hand-react/25-new-user-api)

> 25-new-user-api.mp4

### [前端编写用户注册表单](http://haoqicat.com/hand-in-hand-react/26-signup-form)

> 26-signup-form.mp4

### [前端请求后端 API 完成注册](http://haoqicat.com/hand-in-hand-react/27-signup-done)

> 27-signup-done.mp4

## 第七章：添加管理员功能

### [管理员功能实现](http://haoqicat.com/hand-in-hand-react/28-dashboard)

> 28-dashboard.mp4

### [服务器端实现添加新文章接口](http://haoqicat.com/hand-in-hand-react/29-create-post-api)

> 29-create-post-api.mp4

### [后端限定添加新文章接口的访问权限](http://haoqicat.com/hand-in-hand-react/30-request-auth)

> 30-request-auth.mp4

### [前端实现添加新文章组件](http://haoqicat.com/hand-in-hand-react/31-new-post)

> 31-new-post.mp4

### [前端实现写文章功能](http://haoqicat.com/hand-in-hand-react/32-posts-state)

> 32-posts-state.mp4

### [前端展示新添加的文章](http://haoqicat.com/hand-in-hand-react/33-show-posts)

> 33-show-posts.mp4

### [从服务器端读取所有文章](http://haoqicat.com/hand-in-hand-react/34-show-posts-api)

> 34-show-posts-api.mp4

## 第八章：上传图片功能

### [上传图片组件](http://haoqicat.com/hand-in-hand-react/35-upload-image)

> 35-upload-image.mp4

### [图片保存到服务器并在前端展示出来](http://haoqicat.com/hand-in-hand-react/36-show-image)

> 36-show-image.mp4

## 第九章：单篇文章操作

### [文章操作组件](http://haoqicat.com/hand-in-hand-react/37-post-action)

> 37-post-action.mp4

### [显示文章详情](http://haoqicat.com/hand-in-hand-react/38-show-post)

> 38-show-post.mp4

### [实现编辑文章表单组件](http://haoqicat.com/hand-in-hand-react/39-update-post)

> 39-update-post.mp4

### [完成更新文章功能](http://haoqicat.com/hand-in-hand-react/40-update-post-done)

> 40-update-post-done.mp4

### [实现删除文章功能](http://haoqicat.com/hand-in-hand-react/41-delete-post)

> 41-delete-post.mp4

## 第十章：部署上线

### [PM2 部署项目](http://haoqicat.com/hand-in-hand-react/42-deploy)

> 42-deploy.mp4




















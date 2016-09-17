# [Gulp-Flexbox 响应式网站课程](http://haoqicat.com/gulp-flex-res)

> [采用 gulp 构建工具，flexbox 布局技巧来开发响应式网站，涉及 sass ，google 材料设计，git 和 sublime 技巧。](index.mp4)

搭建 Github 上的一个个人站点。使用 flexbox 技巧设置类似于手机 App 风格的页面布局。走人 Nodejs 生态，实战 npm 装包技巧。上手 gulp 插件系统中最实用的几个插件：图片压缩，布局文件，自动刷新，布局文件套用。练习 google 材料设计这种视觉语言，不会设计的我们也能让页面设计感爆棚。

## 第一章 用 Github 托管网站

### [搭建 Github 个人网站](http://haoqicat.com/gulp-flex-res/1-github-user-site)

参考 <http://pages.github.com> ，可以创建“用户网站”，也可以创建“项目网站”，本视频介绍用户网站的搭建方式。

直接把 html/css/js 存放到 `yourusername.github.io` 这个仓库的 master 分支之上。 这样就可以在 <http://yourusername.github.io> 访问到托管的内容了。

参考[搬进 Github](http://www.imooc.com/learn/390)

### [搭建 Github 项目页面](http://haoqicat.com/gulp-flex-res/2-github-project-site)

代码不能放到 `master` 分支，而要放到 `gh-pages` 分支上。

<http://username.github.io/projectName> 可以看到项目页面了。

### [使用 Coding.net 托管页面](http://haoqicat.com/gulp-flex-res/3-coding-pages)

参考[coding pages 官方帮助](https://coding.net/help/doc/pages/index.html)

## 第二章 安装 nodejs 和 gulp

### [nodejs 为何学？如何学？](http://haoqicat.com/gulp-flex-res/4-nodejs-how)

[npm](https://www.npmjs.com) 包管理器，根据 [nodejs 官网](https://nodejs.org/en/) 上的说法：npm 是世界上最大的开源库生态系统。

[gulp](http://gulpjs.com) 是要比 [grunt](http://gruntjs.com) 更好的前端“构建系统”（ build system ）

### [nodejs 安装](http://haoqicat.com/gulp-flex-res/5-install-node)

推荐使用 nvm 来安装 nodejs, 参考 [nvm 的 README](https://github.com/creationix/nvm) ，执行下面的命令：

`curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.29.0/install.sh | bash`
这样 nvm 就安装好了，可能要重启一下 shell 才有 nvm 这个命令。

查看都有哪些版本可以安装：`nvm ls-remote`
可以看到当前最新版本是 v5.10.1 ，运行下面的命令来安装：

`nvm install v5.10.1`

现在再来安装一个包，看看会被安装到什么位置：

`$ npm i -g gulp`

`/Users/username/.nvm/versions/node/v5.10.1/bin/gulp`
可以看到 gulp 这个包安装到了 /Users/peter 之下。并且可执行文件也自动导出为系统命令了，可以通过运行下面的命令来确认：

`$ which gulp`

`/Users/peter/.nvm/versions/node/v5.10.1/bin/gulp`

设置默认版本

一个小问题，每次启动新 shell ，Node 还是老版本。如何写死成最新安装的 NVM 版本：

`$ nvm alias default 5.10.1`

`default -> 5.10.1 (-> v5.10.1)`

让 npm 使用淘宝镜像

nodejs 安装好之后，npm 这个装包命令也就装好了。npm 命令因为要从国外的服务器下载包，有时候速度不给力，所以这里给一个备选方案：自制一个 cnpm 命令，其实就是一个连接国内淘宝镜像的 npm 命令啦。

参考 [taobao 相关页面](http://npm.taobao.org/)

### [gulp 构建系统](http://haoqicat.com/gulp-flex-res/6-gulp)

先看完这个视频 [好多视频#178《 gulp 构建系统》](http://haoduoshipin.com/v/178)

gulp 是一个构建工具 (build system) ，这里的构建 (build) 主要是指 Web 前端自动化工作流。除了 gulp，还有 grunt，webpack 等其他构建工具。

几个常用的 gulp 插件：

- gulp-autoprefix 自动给 CSS 添加厂商前缀
- gulp-sass 把 Sass 编译成 css
- gulp-imagemin 压缩图片
- gulp-browersync 实现多个设备同步调试，页面自动加载 (live reloading)
- gulp-purifycss 去除没有用的 css 代码
- gulp-wrap 可以把各个 html 文件中相同的 header 和 footer 部分抽离出来

举个例子：

```
gulp.src('src/*.scss') //选取文件
.pipe(sass())
.pipe(prefix())
.pipe(gulp.dest('css/')); //导出到目标文件夹
```

### [使用 gulp-sass](http://haoqicat.com/gulp-flex-res/7-gulp-sass)

## 第三章 gulp 的七十二变

### [sass 的三大功能](http://haoqicat.com/gulp-flex-res/8-sass-use)

参考教程：[sass 使用教程](http://www.sass.hk)，sass 推荐必用的 3 个特性：

- 变量使用
- 嵌套
- 拆分文件


网页设计配色参考：[material Design 色板](https://www.materialpalette.com)

### [autoprefixer 添加厂商前缀](http://haoqicat.com/gulp-flex-res/9-autoprefixer)

可靠的在线[自动添加厂商前缀添加工具](http://autoprefixer.github.io)，安装 `gulp-autoprefixer` 后即可使用。

### [压缩 css 加快页面加载](http://haoqicat.com/gulp-flex-res/10-minify-css)

压缩css文件，安装 `gulp-minify-css` 包。

去除css中没有用到的配置项，安装 `gulp-purifycss` 暂不推荐，可以关注。

### [使用 imagemin 来压缩图片](http://haoqicat.com/gulp-flex-res/11-imagemin)

在不损失图片质量的情况下，压缩图片，推荐使用`gulp-imagemin`这个包。

## 第四章 当材料设计遇到响应式开发

### [为何要移动优先？](http://haoqicat.com/gulp-flex-res/12-mobile-first)

**Mobile First**

### [定制自己的色盘](http://haoqicat.com/gulp-flex-res/13-color-palette)

Github 使用的设计文档，[参考 Primer 开源项目](http://primercss.io/scaffolding/)

[Google Material Design](https://design.google.com/resources/) 视觉设计框架

[Google polymer project](https://www.polymer-project.org/1.0/) 提供 web component 设计

Material Design 素材库参考: [material up](https://material.uplabs.com)

Material Design 素材库参考：[@dirbbble](https://dribbble.com/search?q=material+design)

开始 material design 的第一步，定制自己的[色盘](http://haoqicat.com/gulp-flex-res/13-color-palette)

### [色盘上各种颜色的作用](http://haoqicat.com/gulp-flex-res/14-colors-how)

- primary color：主题色
- accent color: 按钮、表单、突出显示 等
- text/icon color：主题色上面的文字、icon颜色，白色为主
- primary text color：白色背景上的文字颜色，主要是黑色
- secondray text color: 比 primary color 浅
- divider color: 分隔线的颜色
- dark primary color: 深主题色
- light primary color: 浅主题色

### [什么是响应式设计](http://haoqicat.com/gulp-flex-res/15-responsive-design-what)

响应式三要素:

1. 弹性布局；
2. 弹性图片；
3. media 查询。

### [四种常见响应模式](http://haoqicat.com/gulp-flex-res/16-responsive-patterns)

- Column Drop 列下沉
- Mostly Fulid 基本流体式
- Layout Shifter
- Off Canvas 抽屉式

### [viewport 设置](http://haoqicat.com/gulp-flex-res/17-viewport)

常用设置：

`<meta name="viewport" content="width=device-width, initial-scale=1">`

## 第五章 Flexbox 来了

### [flexbox 时代来临](http://haoqicat.com/gulp-flex-res/18-flexbox-here)

flexbox 学习资源:

- <https://scotch.io/tutorials/a-visual-guide-to-css3-flexbox-properties>
- <https://teamtreehouse.com/library/css-flexbox-layout/understanding-flexbox/flexbox-basics-and-terminology>
- <http://flexbox.io>
- <http://www.fullstackradio.com/24>

### [项目准备](http://haoqicat.com/gulp-flex-res/19-get-ready)

全部代码：<https://github.com/happypeter/flex/commit/886ad68d0c564b576b9059412f95b7e9a1263295>

### [类似手机 app 的移动版布局](http://haoqicat.com/gulp-flex-res/20-app-layout)

全部代码：<https://github.com/happypeter/flex/commit/b07def076c6673bc5d3da597c3d6bba20c287e67>

参考资料：

- <http://flexbox.io>
- <https://css-tricks.com/snippets/css/a-guide-to-flexbox/>

### [使用 font-awesome 图标](http://haoqicat.com/gulp-flex-res/21-font-awesome)

全部代码：<https://github.com/happypeter/flex/commit/e99a2252e57a5dd253338b4dd1cd4d368988e1ae>

### [gulp-wrap 使用布局文件](http://haoqicat.com/gulp-flex-res/22-gulp-wrap)

全部代码：<https://github.com/happypeter/flex/commit/6d2787238902cc60ebb5924f782c45c7310eb8b9>

### [browser-sync 页面自动刷新](http://haoqicat.com/gulp-flex-res/23-browsersync)

全部代码：<https://github.com/happypeter/flex/commit/20f4f7d8443e3c37cd150d8979d1eebcd8eac520>

## 第六章 Media 查询

### [使用 media query](http://haoqicat.com/gulp-flex-res/24-media-query)

根据网站的内容选择最佳临界点

可以参考bootstrap中对于临界点的设置

基本代码如下：

```
@media(min-width: 600px){
	...
}
```

按照移动优先的设计思路，min-width 会覆盖几乎所有的使用场景，而 max-width 几乎可以不用。

参考 [google develops](https://developers.google.com/web/fundamentals/design-and-ui/responsive/fundamentals/how-to-choose-breakpoints?hl=en#pick-minor-breakpoints-when-necessary) 的这篇文章。

### [响应式导航](http://haoqicat.com/gulp-flex-res/25-res-nav)

本节代码：[res-nav](https://github.com/happypeter/flex/commit/41ec2a56211066fdfdfd90dcca419359a3633990)

### [flexbox 制作流体网格](http://haoqicat.com/gulp-flex-res/26-flex-grid)

- 拆分 scss 代码
- 设置 media-query
- 参考代码：[flex-grid](https://github.com/happypeter/flex/commit/5c90c6b434a89df295f1f2fb1518e93159d41ce0)

### [总结](http://haoqicat.com/gulp-flex-res/27-end)

代码：

- [stage1-end](https://github.com/happypeter/flex/commit/6268fa739a92d59a1bddda53bfb644f877e6e0d4)
- [fix img path](https://github.com/happypeter/flex/commit/14e74e7fb03c15a75abd0ec8cdbfc3eab2582e4a)


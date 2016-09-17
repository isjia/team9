# [Flexbox 舞娘](http://haoqicat.com/flexbox-dancer)

> 还在学习 float 和 clearfix 技巧来设置布局吗？你可能正在浪费自己的时间哦

折腾过 float/clearfix 这些技巧的老手有福气了，不用再折腾了。没有折腾过 float 的新手当然更有福气了，因为不用走弯路了。学习 React Web 开发，flexbox 是最明智的布局技巧，使用 React Native 开发，flexbox 就是官方默认技巧。

真正的 Flexbox 入门课程，先来聊浏览器兼容，然后聊各个属性的具体作用，进一步上综合性强一些的实用案例，帮助大家在脑子中建立起用 flexbox 进行布局的一个思维模型。

## 第一章 基础部分

### [为何 Flexbox 时代已经到了](http://haoqicat.com/flexbox-dancer/1-flexbox-why)

[css-tricks 上的 flexbox 指南](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

浏览器兼容性：[canIuse flexbox](http://caniuse.com/flexbox), 95%以上浏览器都可以支持

### [flex-direction 排列方向](http://haoqicat.com/flexbox-dancer/2-flex-direction)

flex direction 应该是 flexbox 所有知识点中最基础的一个了，总结起来就是一句话：

> 对 flex item 的排列方向做控制。

核心代码：

```
.parent {
  display: flex;
  flex-direction: column;
}
```

参考资料

- [What Flexbox](http://haoqicat.com/flexbox-dancer/flexbox.io)

### [felx-wrap 控制换行](http://haoqicat.com/flexbox-dancer/3-flex-wrap)

允许换行的写法：

```
.parent {
  ...
  flex-wrap: wrap;
}
```

### [justify-content 对齐方式](http://haoqicat.com/flexbox-dancer/4-justify-content)

> flexbox 的 justify-content 技巧用来控制元素的对齐方式。

示例代码：

```
.parent {
  justify-content: space-between;
}
```

### [flex 属性](http://haoqicat.com/flexbox-dancer/5-flex)

示例代码：

```
.box {
  flex: 1;
}

.second {
  flex: 2;
}
```

### [flex 属性对应的三个属性](http://haoqicat.com/flexbox-dancer/6-flex-3)

- flex-grow
- flex-shrink
- flex-basis

## 第二章 实用案例

### [三栏布局](http://haoqicat.com/flexbox-dancer/7-demo1)

参考: <https://www.youtube.com/watch?v=H1lREysgdgc>

### [流体布局](http://haoqicat.com/flexbox-dancer/8-demo2)

## 第三章 Goodbye

### [更多学习建议](http://haoqicat.com/flexbox-dancer/9-goodbye)

- [MDN 使用 CSS 弹性盒子](https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes)
- [CSS-tricks 的文章](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- <http://flexbox.io/>




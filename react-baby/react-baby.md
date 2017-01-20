# [React 婴儿](http://haoqicat.com/react-baby)

这么可不讲 npm/wepack/api/reudx 等，专注介绍React本身的核心概念。学习React的属性、状态机制、生命周期、事件响应等核心知识。

## 第一章：概述

### [React 游戏规则改变着](http://haoqicat.com/react-baby/1-react-show)

一切皆组件：组件把数据翻译成UI。数据通过组件的 props 属性传入，组件资深状态通过 state 状态值来控制。数据有变化，组件马上自动刷新。

**React 组件化带来的颠覆：**

- 分离 html/CSS
- 非侵入式 js
- 以 ploymer 为代表的传统组件
- jQuery
- 模板及内嵌语言
- MVC
- CSS
- Bootstrap

**React 带来的新思路**

- 提高内聚：用于实现统一功能的代码将被放置到一起
- 降低外联：不因为其他组件的失效而影响

## 第二章：关键技术点

### [Hello World](http://haoqicat.com/react-baby/2-react-hello-world)

### [传递属性值](http://haoqicat.com/react-baby/3-react-props)

### [Children](http://haoqicat.com/react-baby/4-react-children)

### [事件响应](http://haoqicat.com/react-baby/5-react-event)

### [State 状态值](http://haoqicat.com/react-baby/6-react-state)

### [生命周期](http://haoqicat.com/react-baby/7-react-lifecycle)

1. 初始化
  - 获取默认属性值 getDefaultProps()
  - 获取实例初始状态 getInitialState()
  - 首次渲染之前 componentWillMount()
  - 渲染 render()
  - 首次渲染之后 componentDidMount()

2. 更新
  - 属性被修改前 componentWillReactiveProps()
  - 判断是否需要更新 shouldComponentUpdate()
  - 更新之前 componentWillUpdate()
  - 渲染 render()
  - 更新之后 componentDidMount()

3. 销毁
  - 销毁前 componentWillUnmount()

更多信息 google “React Lifecycle"

## 第三章： Goodbye

### [进一步学习](http://haoqicat.com/react-baby/8-more)



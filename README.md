# Mini-Vue3
一个迷你版的Vue3框架，帮助更多人以更简单的方式学习vue 3源码


## 前言
在很早之前学习完Vue的时候，就对Vue的神奇之处赞叹非常，之后又读了Vue.js 设计与实现这本书，对Vue的低层实现原理更是愈发好奇。
但是因为初出茅庐，一直没有机会也没有实力去学习Vue源码知识。
直到前段时间，认识了Sunday老师，听了老师的源码课，终于结束了萌新时期对Vue低层实现的好奇和向往，完成了对Vue源码知识的学习，并且自己手写了一个简单Mini版的Vue3框架。
在这里，我把它分享出来，希望能帮到更多的人，以一种更简单的方式学习Vue3 源码。（PS：不用担心看不懂，基本每一行代码都有注释，只要你懂一些TS，就完全没问题）


## 基本介绍
Mini-Vue3中主要包括的核心模块如下：
1，响应性
2，运行时
其中运行时包括：运行时核心和 运行时dom
3，编译器
编译器部分比较复杂，另外用处并不多，所以这里根据项目里的 编译器文档 仅作了解即可


## 开发标准
**没有使用的代码就当做不存在**
因为在vue的源码中，它会存在很多边缘情况的处理。比如：
用户提交的数据不符合规定，那么应该提交什么类型的错误，不同类型提交的错误内容同样不一样。
像这种关联核心逻辑的边缘情况，我们认为它们不存在，从而使我们更加关注核心逻辑，避免陷入复杂的逻辑循环处理。


**用的最少代码实现核心逻辑**
针对指定的业务场景，来构建最清晰的实现路径。
因为避免了很多的边缘情况，所以这可以保证在实现的时候，完全专注于核心业务，业务的更多关注，就意味着业务的更加严格。从而以最小的学习成本来达到最大的学习收益。


## 运行
使用npm进行安装依赖：
  npm i
运行项目：
  npm run dev

测试实例查看packages/vue/examples

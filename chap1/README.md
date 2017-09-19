# 第一章： Electron简介
Node.js是用JavaScript开发服务端web应用的开源、跨平台运行环境。它用Google的V8引擎来解释执行JavaScript。
非常多的web框架诸如Express和Hapi都可在Node.js中使用。现如今，它是标准软件开发生态圈使用较为普遍的工具。
例如，绝大部分客户端JavaScript框架使用Node.js来自动化开发过程，诸如构建、压缩JavaScript、编译源码等等。
但是绝大部分人对node仅能在web应用和命令行实用程序发挥作用的认知是错误的，事实是我们可以使用Node.js做几乎任何其他编程语言和平台能做的所有事情。

在本书中，我们将谈论如何使用Node.js来构建可以运行在所有主流操作系统上的桌面应用。
你可能对这个组合-JavaScript和桌面应用感到困惑。你可以在你的日常生活中使用这种类型的应用。
你在工作中使用过[Slack][1]吗？又或者你在编辑你的源码时，是否正在使用Github Atom编辑器或Microsoft Visual Studio Code？
那么你已经使用过基于Node.js的桌面应用了。这些都是典型的基于Node.js的桌面应用。

在使用Node.js和web技术构建桌面应用时，有两个主要的可选项：
- NW.js(曾用名：node-webkit)
- Electron(曾用名：atom shell)

两个框架都是开源的，并被诸如Intel和Github等大企业所支持。两者都拥有庞大的社区。

在本书中，我们将会探讨使用Github Electron框架构建桌面程序。在我们开始应用开发前看看Electron内部构造。
本章中，我们将会谈论以下要点：
- Electron的简史和介绍
- Electron相较于传统桌面应用的优势
- 用Electron构建一个Hello World应用
- 用Electron集成Node.js环境到web页面
- electron内部构造

## 第一节 为什么是桌面应用？
软件在过去几年中发生了巨大的变化。在最近几十年的开始，绝大部分软件都是桌面应用。但是随着时间变迁，web慢慢占据了优势。
随着Ajax的出现，再次推动着web到达新的时代。在Internet上所有的事物都变成分布式的。云计算物联网推动着软件技术到达下一个阶段并扩展至多媒体设备。

那么，我们真的需要开发桌面应用吗？我们并不能完全去掉桌面应用。即使世界的趋势云计算和web技术，我们在有些条件下仍然需要桌面程序：
- 当数据安全是必要的，并且数据不能通过Internet曝光，那么桌面应用是最佳选择。
- 当你的应用需要通过操作系统组件和基础硬件时。
- 当你需要开发各种工具应用，诸如IDE、编辑器等等

当然，还有很多条件下只能使用桌面应用。但是构建一个能在大多数操作系统运行的应用永远都是个挑战。


[1]: https://baike.baidu.com/item/slack/4264540?fr=aladdin
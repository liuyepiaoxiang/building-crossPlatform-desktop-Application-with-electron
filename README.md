# 前言


## 版权所有
本书的任何一部分在未经出版者事先书面许可时不能被复制、保存在任何一个检索系统内，或者用任何形式和方式进行传播。评论文章或短语引用除外。

## 关于作者
加西姆·穆罕默德在企业参与WEB应用项目的时间已逾8年。从Microsoft.NET平台开始他的软件开发生涯，现在以全栈工程师的身份开发JavaScript应用。
在他的工作生涯中，他开发了很多.NET和Node.js平台的大量的技术和框架的项目。目前他在迪拜的一家航空公司就职，并专注于全栈JavaScript应用开发。

我非常感谢我的妻子，Fathima，在本书成书期间表现她的爱、善良以及支持。同时感谢我的父母无尽的爱意和支持。

## 关于评论家
安德鲁·帕罗迪以专家级软件开发者身份工作已逾20年。他在职业生涯中擅长多种语言和技术。
去年期间，他使用JavaScript和web平台为一个大型软件公司开发手机应用。
在过去的年月，他开始持续在Github为electron开源社区、公开库贡献智慧。

非常感谢我的妻子，塔提亚娜，在本书审稿期间用她的耐心和珍贵的建议帮助我。

# 简介
## 序
本书指导读者通过使用GitHub Electron框架构建能在Windows、Mac和Linux平台上运行桌面程序。本书描述了如何用你已有的web开发技巧来构建一个使用HTML、CSS和JavaScript的跨端桌面应用。

Electron是一个非常流行的使用JavaScript和Node.js创建跨端桌面应用的框架。它在Google的chromium项目上构建。现在，在公司和开发者们中，越来越流行使用它来创建他们的产品。

在本书中，我们将讲述从安装工具、编写应用、使用Electron结合各种各样的第三方工具和框架的方方面面。

## 本书概览
[第一章](chap1/README.md),Electron简介,Electron的基本概览及解释Electron的内部机制。本章我们将了解Electron如何运行及其内部构造。

[第二章](chap2/README.md),创建第一个Electron应用,谈论一步步指导开发一个应用，包括创建一个简单应用从环境设置到运行应用的所有步骤。

[第三章](chap3/README.md),工具和调试,包括工具和调试应用。提供如何使用各种各样可用的工具和IDE来调试应用的详尽的方法。

[第四章](chap4/README.md),使用Angular2与Electron,解释使用Angular2和TypeScript来创建用户界面的Electron应用。本章也将谈论一些新技术趋势。
并提供如何使用现代前端框架和技术与Electron应用结合的详尽方法。

[第五章](chap5/README.md),设计用户界面,展示如何为Electron创建用户界面。本章内容包括各种各样的UI框架以及一些基于Electron的UI框架，例如Photon；
如何使用流行的React框架来为你的Electron应用创建用户界面。

[第六章](chap6/README.md),使用Node.js与Electron,教你如何在你的Electron项目内使用Node.js环境。本章将提供在Electron应用内使用Node.js的API完整的指导。

[第七章](chap7/README.md),深入研究ElectronAPI-1,Electron API介绍。本章将介绍诸如Clipboard、Process、Shell、Image、File、Dialog、Accelerator以及Session等Electron APIs。
也包括一些高级主题，如请求拦截和自定义协议实现等。

[第八章](chap8/README.md),探索ElectronAPI-2,继续探索Electron APIs。本章将包括一些高级特性，如用来控制渲染进程的webContents API、Chrome命令行转换器以及下载API等等。

[第九章](chap9/README.md),结合桌面环境,不同操作系统在其桌面环境结合桌面应用的不同显示特性。本章将解释如何如何在桌面环境中用electron APIs结合我们的应用。

[第十章](chap10/README.md),Web标准化处理,关注如何让Electron与各种web标准结合。本章包括的主题，诸如使用service worker、local storage缓存网络资源、使用IndexedDB持久化数据。

[第十一章](chap11/README.md),测试Electron,展示测试是软件应用开发过程中非常重要的部分。本章主要包括测试你的electron应用、如何使用流行的JavaScript测试框架以及如何在electron应用内使用这些框架。

[第十二章](chap11/README.md),打包和分发应用,解释如何为最终产品打包应用。本章包括打包和分发我们的应用需要的各种库，描述如何为每个平台移植本地包，如何在有更新时自动更新，创建ASAR包，为每个平台创建安装软件以及各大应用商店的上线指导。

## 阅读本书前的准备
- 一个文本编辑器来创建HTML、CSS和JavaScript文件；你也可以使用你钟意的编辑器。
- 安装版本4.x及以后或最新的Node.js的系统，推荐使用至少6.x及之后的版本。
- 一个包管理器，诸如npm或者yarn；npm将会在Node.js安装过程中默认安装。
- （可选）安装Git客户端的电脑，如果你需要从我们的Git仓库直接check out源码。

## 该书读者群
如果你是一个对HTML、CSS和JavaScript比较熟悉的开发者，并且希望开发用上述技术开发桌面应用，那么本书是为你而写的。
本书也是为那些有经验的JavaScript开发者并对前端开发和Node.js开发有基础了解的开发者而写。
本书也适合那些想用他们开发web开发中的技术开发一款桌面应用的前端/web开发者。

## 约定
在本书中，你将看到一些特殊的文本样式，下面是这样样式及其解释。

代码片段，数据库表名，文件夹名称，文件名，文件扩展名，路径名称，虚拟URLs，用户输入，以及推特链接将如下显示：Electron then loads the HTML page using the `loadurl` function。
代码块如下：
```js
{
  "name"    : "your-app",
  "version" : "0.1.0",
  "main"    : "main.js"
}
```

任何命令行输入和输出如下：
```git
 curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
 sudo apt-get install -y node.js
```
**新的表达方式**和**重要词语**将用粗体展示。在屏幕上看到的句子，例如，在菜单中或者对话窗口，出现在被引用的文本环绕，或者像这样：Just hit the Download button and click OK.

![img](img/info.png)出现在框内的警告或者重要提示像这样。

![img](img/tip.png)提示和诀窍像这样。



## 说明
本书为本人在业余时间翻译，因本人专业水平和翻译水平有限，导致翻译不尽人意，还望见谅，还望您提供宝贵的修改意见帮助一同改善本书的质量，谢谢！
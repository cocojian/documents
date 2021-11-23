---
title: "Day01-概述 安装 配置"
date: 2021-11-22T21:30:31+08:00
draft: false
tags: ["flutter"]
categories: ["flutter"]
---


（一）Flutter概述

* * *
Flutter是谷歌的移动UI框架，使用dart语言来编写，可以快速在iOS和Android上构建高质量的原生用户界面。 Flutter可以与现有的代码一起工作。在全世界，Flutter正在被越来越多的开发者和组织使用，并且Flutter是完全免费、开源的。

Flutter Widget采用现代响应式框架构建，这是从 React 中获得的灵感，**中心思想是用widget（组件）构建你的UI**。 当widget的状态发生变化时，widget会重新构建UI，Flutter会对比前后变化的不同， 以确定底层渲染树从一个状态转换到下一个状态所需的最小更改（译者语：类似于React/Vue中虚拟DOM的diff算法。

最新的版本是2.2
  

* [flutter 官网 （网络不太稳定）](https://flutter.dev/)
* [flutter中文网](https://flutterchina.club/)
* [flutter插件下载](https://pub.dev/)

* * *

（二）Flutter优点

1. **效率** Flutter的热重载可帮助您快速地进行测试、构建UI、添加功能并更快地修复错误。在iOS和Android模拟器或真机上可以在亚秒内重载，并且不会丢失状态。
2. **美观** 使用Flutter内置美丽的Material Design和Cupertino（iOS风格）widget、丰富的motion API、平滑而自然的滑动效果和平台感知，为您的用户带来全新体验。
3. **多终端** 使用Flutter的现代、响应式框架，和一系列基础widget，轻松构建您的用户界面。使用功能强大且灵活的API（针对2D、动画、手势、效果等）解决艰难的UI挑战。
4. **访问本地功能和SDK** 通过平台相关的API、第三方SDK和原生代码让您的应用变得强大易用。 Flutter允许您复用现有的Java、Swift或ObjC代码，访问iOS和Android上的原生系统功能和系统SDK。

* * *
（三）Flutter安装

1. 去flutter官网下载其最新可用的安装包，[点击下载](https://flutter.dev/docs/development/tools/sdk/releases#windows) 。在中国大陆地区，要想正常获取安装包列表或下载安装包，可能需要翻墙，读者也可以去Flutter github项目下去[下载安装包](https://github.com/flutter/flutter/releases) 。
2. 将安装包zip解压到你想安装Flutter SDK的路径（如：C:\src\flutter；注意，不要将flutter安装到需要一些高权限的路径如C:\Program Files\。
3. 由于在国内访问Flutter有时可能会受到限制，Flutter官方为中国开发者搭建了临时镜像
    1. 到 “控制面板>用户帐户>用户帐户>更改我的环境变量”
    2. 在“用户变量”下检查是否有名为“Path”的条目:如果该条目存在, 追加 flutter\bin的全路径，使用 ; 作为分隔符.如果条目不存在, 创建一个新用户变量 Path ，然后将 flutter\bin的全路径作为它的值.
    3. 在“用户变量”下添加两个变量
    PUB_HOSTED_URL=https://pub.flutter-io.cn
    FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn
 4. 打开一个新的命令提示符或PowerShell窗口并运行以下命令以查看是否需要安装任何依赖项来完成安装：flutter doctor

* * *
（三）IDE安装

1.下载并安装 Android Studio.
2. 启动Android Studio，然后执行“Android Studio安装向导”。这将安装最新的Android SDK，Android SDK平台工具和Android SDK构建工具，这是Flutter为Android开发时所必需的
3. Flutter插件： 支持Flutter开发工作流 (运行、调试、热重载等).
4. Dart插件： 提供代码分析 (输入代码时进行验证、代码补全等).

* * *

（四）模拟器安装

1. 使用Android Studio内置安卓模拟器
2. 使用真机

* * *

（五）创建flutter工程

1. 选择 File>New Flutter Project选择 Flutter application 作为 project 类型, 然后点击 Next输入项目名称 (如 myapp), 然后点击 Next点击 Finish等待Android Studio安装SDK并创建项目
2. 上述命令创建一个Flutter项目，项目名为myapp（可以为任意的名称），其中包含一个使用Material 组件的简单演示应用程序。在项目目录中，您应用程序的代码位于 lib/main.dart.
3. 运行应用程序
![Local Picture](/Image.png "Local Picture")
4.  热重载（hot reload） 对代码进行更改，然后告诉IDE你需要重新加载（点击reload按钮），你就会在你的设备或模拟器上看到更改。



---
title: 如何集成插件图表
---

## 1. 如果你是一位使用者

1. 从`dist`文件夹中拷贝出你所需要的插件图表，如`datart-amap.iife.js`这个给予高德地图的插件图表
2. 将拷贝出的插件图表粘贴到你的datart服务端的`custom-chart-plugins`目录下
3. 登陆 datart 系统，然后选择你所导入的插件图表

## 2. 如果你是一位开发者

> 当前的仓库提供了基于命令行的工具，提升开发效率。

### 2.1. 制作 IIFE 类型的插件图表 （推荐）

> 立即调用函数表达式（英文：immediately-invoked function expression，缩写：IIFE）[1]，是一种利用JavaScript函数生成新作用域的编程方法。

1. 创建一个以`datart-`开头的文件夹，如`datart-hello-world`文件夹
2. 创建一个 **Javascript** or **Typescript** 文件
3. 导出一个包含 datart 生命周期的函数对象，生命周期[^2]例如`onMount`、`onUpdated`等.
4. 运行`npm run build` 命令，并且查看`dist`文件夹新生成的`datart-hello-world.iife.js`文件

**注意：插件图表文件夹的名称必须以`datart-`开头，这样当运行build命令时可自动打包文件**

### 2.2. 制作 React 类型的插件图表

**请查看`plugins`文件夹📁下面的图表示例**

插件图表仓库地址请访问：[这里](https://github.com/running-elephant/datart-extension-charts)

## 3. 更多文章链接

- [x] Plugin Chart Helper API document: <https://running-elephant.github.io/datart-docs/api/>
- [x] How to Make a Plugin Chart: <https://running-elephant.github.io/datart-docs/docs/chart_plugin.html>
- [x] How to Make Chart Config: <https://juejin.cn/post/7040683275446124574>
- [x] Vue 跑马灯插件示例: <https://mp.weixin.qq.com/s/a4DVf-5LHVQAknmKKE6DJA>
- [x] JQuery 图表插件：<https://mp.weixin.qq.com/s/9hBNSla86Fzouy0WdXqSQQ>
- [x] 手把手教你开发出优秀的图表插件作品： <https://mp.weixin.qq.com/s/nYMAaiT97NPkm71FpW8LSw>

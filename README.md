# 说明

> A Mpvue project

    "node": ">= 4.0.0",
    "npm": ">= 3.0.0"，
    "mpvue-loader": "1.0.13"

## 项目目录结构

>src 项目目录
>
>apis 接口管理
>
>components 通用组件
>
>config 通用数据
>
>pages 页面
>
>>taskList 任务板块相关
>>
>>talkTopic 话题板块相关
>>
>>create 创建板块相关
>>
>>activity 活动板块相关
>>
>>personCenter 我的板块相关
>>
>>authorize 全局拦截授权
>>
>store 状态管理
>
>utils 后期整合到 config 内
>
>static 项目静态资源目录

## 项目运行（nodejs 4.0+）
``` bash

# 安装Node.js
sudo apt-get install nodejs
sudo apt-get install npm

# 克隆到本地
git clone https://gitee.com/ezi/qbxcx.git

# 进入文件夹
cd qbxcx

# 安装依赖
npm install

# 开启本地服务器localhost:8080
npm run dev

# 发布环境
npm run build
```

## 开发前环境搭建
### 1. 开发工具下载
首先在微信官网上下载[微信开发者工具](https://developers.weixin.qq.com/miniprogram/dev/devtools/download.html)。利用微信开发者工具，开发者可以完成小程序的 API 和页面的开发调试、代码查看和编辑、小程序预览和发布等功能。

推荐使用Visual Studio Code作为文本编辑器， 当然也可使用其他喜欢的编辑器。
### 2. 创建项目
打开开发者工具，选择“导入项目”，选取目录为编译后生成的dist目录，填写如同所示的AppID。只有填写了合法的AppID才能使用微信提供的高级接口。

<img src='https://github.com/Ashley713/qbxcx/blob/master/import.jpeg'>

然后导入项目，点击工具栏-编译，就能在左边的模拟器中看到小程序的运行效果。

<img src='https://github.com/Ashley713/qbxcx/blob/master/demo.jpeg'>

## 本地调试
### 1. 模拟器调试
在本地服务器开启状态下，当更改项目文件时，npm会自动重新编译并刷新模拟器。此时可在左侧的模拟器中即时查看运行效果。
### 2. 真机调试（推荐）
点击工具栏-真机调试，微信扫描二维码后即可在手机上查看小程序的运行效果。只能在绑定了微信开发者的微信号上进行真机调试。

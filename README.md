# ***ControlerHost*** **使用手册**  

- [***ControlerHost*** **使用手册**](#controlerhost-使用手册)
  - [适用范围](#适用范围)
  - [主要特性](#主要特性)
  - [安装环境](#安装环境)
  - [硬件环境](#硬件环境)
  - [安装方式](#安装方式)
  - [功能详述](#功能详述)
    - [标题栏](#标题栏)
    - [导航栏\&工作区](#导航栏工作区)
      - [校准对零](#校准对零)
      - [固件生成](#固件生成)
      - [IAP升级](#iap升级)
      - [BiSS调试](#biss调试)
    - [状态栏](#状态栏)
    - [特别说明](#特别说明)
- [***ControlerHost***](#controlerhost)
---
---
---


## 适用范围

- [ONK-深圳欧诺克科技有限公司](https://www.sz-onk.com/) `LME` 系列编码器;
- [ONK-深圳欧诺克科技有限公司](https://www.sz-onk.com/) `AbsReslover` 旋变解析卡;
- [ONK-深圳欧诺克科技有限公司](https://www.sz-onk.com/) `BiSS-Master` 调试板；
- [ONK-深圳欧诺克科技有限公司](https://www.sz-onk.com/) `Calibration Controler` 校准工装；

## 主要特性  

- 支持 `LME` 系列编码器[校准调零](#校准调零)； 
- 支持 `LME` 与 `AbsReslover` [参数配置与调试]();
- 支持 `LME` 、 `AbsReslover`、 `BiSS-Master` 、`Calibration Controler`系列产品[固件升级]()；

## 安装环境

- 系统 `Windows x64` / `Windows x86`;
- 串口驱动[CH340/CH341](https://www.wch.cn/downloads/CH341SER_EXE.html);
  
## 硬件环境

- 对`LME`编码器的[校准调零](#校准调零)： 需要配备[ONK-深圳欧诺克科技有限公司](https://www.sz-onk.com/) `Calibration Controler` 校准工装；
- 对 `LME` 与 `AbsReslover` [参数配置与调试]()： 需配备[ONK-深圳欧诺克科技有限公司](https://www.sz-onk.com/) `BiSS-Master` 调试板;
- 对 `LME` 与 `AbsReslover` [固件升级](#固件升级)： 需配备[ONK-深圳欧诺克科技有限公司](https://www.sz-onk.com/) `BiSS-Master` 调试板;

## 安装方式

- 在线安装方式：[在线安装包下载地址](https://hsguy-y.github.io/ONK_Release/ControlerHost/install/onk_controlerhost_online_install.exe);
- 离线安装方式：[离线安装包下载地址](https://hsguy-y.github.io/ONK_Release/ControlerHost/install/onk_controlerhost_offline_install.exe);

## 功能详述

*详细介绍此应用的各项功能，操作方式。*

### 标题栏

1. ***文件***<br>

   *文件选项卡，主要提供对 `.bin` 文件的`新建`、`打开`、`修改`、`保存`等操作。*<br>

    - ***打开 `.bin` 文件；***<br>
      - ***点击 `文件` -> `打开固件`***<br>
        <img src ="./screenshot/open_bin01.png" width="620"/><br>
      - ***选择 `.bin` 文件；***<br>
        <img src ="./screenshot/open_bin02.png" width="620"/><br>
      - ***浏览或编辑 `.bin` 文件。***<br>
        <img src ="./screenshot/open_bin03.png" width="620"/><br>
    - ***保存 `.bin` 文件***<br>
      - ***点击 `文件` -> `保存`（<kbd>Ctrl</kbd> + <kbd>S</kbd>）或 `文件` -> `另存为`（<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>S</kbd>）均可保存文件。***<br> 
        <img src = "./screenshot/save_bin.png" width ="620" /><br>

2. ***连接***<br>

   *连接选项卡，可用于不同设备的`链接`操作。*<br>

    - ***点击 `连接` -> `串口`；***<br>
        <img src = "./screenshot/connect01.png" width = "620"/><br>
    - ***选择 `串口号` 、 `波特率` 、`设备型号`；***<br>
        <img src = "./screenshot/connect02.png" width = "620"/><br>
    - ***成功连接`指定设备`；***<br>
        <img src = "./screenshot/connect03.png" width = "620"/><br>

3. ***设置***<br>
   
   1. ***权限设置***<br>
    
        *本软件通过用户权限不同提供不同的功能选项;*<br>
    
        *权限角色分为：<kbd>用户</kbd>、<kbd>调试员</kbd>、<kbd>管理员</kbd>；*<br>
       - ***可通过标题栏中 `设置` -> `权限设置` 中修改用户权限。***<br>
            <img src="./screenshot/userpremiss01.png" width = "620" /><br>
       - ***选择权限 `用户` ，输入 [密码]()***<br>
            <img src="./screenshot/userpremiss02.png" width = "620" /><br>
       - ***切换至`用户权限`***<br>
            <img src="./screenshot/user.png" width = "620" /><br>

   2. ***语言设置***<br>
   
        *应用支持多种语言切换。注意：（语言切换均基于<kbd>中文机翻</kbd>）；*<br>

       - ***可通过标题栏中 `设置` -> `语言设置` 中修改语种***<br>
            <img src = "./screenshot/languag01.png" width = "620"/><br>
       - ***选择语言 `英文`，点击`确认`***<br>
            <img src = "./screenshot/languag02.png" width = "620"/><br>
       - ***切换至`英文页面`***<br>
            <img src = "./screenshot/english.png" width = "620"/><br>

4. ***设备***<br>
   
   *设备选项卡，用于拓展`新设备`，添加新设备参数以适配程序功能<mark>（用户权限下无法使用）</mark>。*<br>
   - ***点击 `设备` -> `添加设备`；***<br>
        <img src = "./screenshot/devices01.png" width = "620"/><br>
   - ***添加 `设备参数`;***<br>
        <img src = "./screenshot/devices02.png" width = "620"/><br>
   - ***添加成功,可在 `设备类型` 中找到添加的设备 `onk_test001`；***<br>
        <img src = "./screenshot/devices03.png" width = "620"/><br>

### 导航栏&工作区

*导航栏包含应用各项功能的`导航目录`；其与工作区各项功能项相互连接，可通过点击目录导航至对应`功能选项`。*
#### 校准对零

#### 固件生成
#### IAP升级
#### BiSS调试
### 状态栏

*应用底部状态栏：包含`调试信息`显示按钮、`进度条`；用于提示耗时操作`进度`，以及程序`运行状态`。*

   - ***点击左下角 <kbd><img src= "./icons/message.png"/></kbd> 图标， 可打开`调试信息`窗口***<br>
        <img src= "./screenshot/status.png" width = "620"><br>
   - ***`调试信息`界面，再次点击左下角 <kbd><img src= "./icons/message.png"/></kbd> 图标，可隐藏`调试信息`窗口***<br>
        <img src= "./screenshot/status01.png" width = "620"><br>
   - ***`错误`状态下`状态栏样式`***<br>
    <img src= "./screenshot/status02.png" width = "620"><br>
   - ***操作`成功`状态下`状态栏样式`***<br>
    <img src= "./screenshot/status03.png" width = "620"><br>

### 特别说明

 




# ***ControlerHost***
<img src ="https://hsguy-y.github.io/ONK_Release/icons/set.png" width ="180" height= "180" align = center/>
<img class = "img-container" src ="https://www.sz-onk.com/picture/logo.png" width ="180" height= "40" align = center/>



![](https://img.shields.io/github/stars/HsGuy-Y/ONK_Release.svg)
![](https://img.shields.io/github/forks/HsGuy-Y/ONK_Release.svg)
![](https://img.shields.io/github/issues/HsGuy-Y/ONK_Release.svg)
![](https://img.shields.io/github/tag/HsGuy-Y/ONK_Release.svg)
![](https://img.shields.io/github/release/HsGuy-Y/ONK_Release.svg) 

<style>
.img-container{
    background-color: #333 !important;
    max-width:100;
    height:40;
    padding:0;
    margin:0;
}   
</style> 

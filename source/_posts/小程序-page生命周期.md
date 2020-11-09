---
title: 小程序-page生命周期
date: 2020-11-09 11:00:58
tags: 微信小程序
# thumbnail: 
---

#### onload
【进入页面加载，页面加载时发生，只发生一次】
进入页面，刷新页面，页面销毁后再次进入都会触发


#### onShow
 【页面显示，就会调用】
初次进入onLoad触发后会触发onShow，从后台恢复会触发，页面回退，授权后重新切入，都会触发

#### onReady
【页面初次渲染会触发】
只有初次渲染时触发，只触发一次
例如对界面的设置如wx.setNavigationBarTitle请在onReady之后设置

#### onHide
【页面隐藏】
当前页切入后台，或者进入到别的页面触发

#### onUnload
【页面卸载】
当前页回退，当redirectTo或navigateBack的时候调用

![image.png](https://upload-images.jianshu.io/upload_images/21448083-de5829dacf49e7f2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

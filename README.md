# floatButton
小程序 可拖动悬浮按钮 已封装成模块可直接引用
https://github.com/suzhixiaoliao/floatButton/blob/master/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20190110160957.png

# 步骤一
 const FloatButton = require('../../template/floatButton/floatButton.js')
 var floatButton;
     floatButton = new FloatButton(this, "home", {
       image: "../../assets/jq/home.png",//图像路径，必须
      onclick: function () {
       wx.showToast({
          title: 'fb click 1',
        })
     },
     imageRadio: 1,
     imageWidthRadio: 0.1,
       onLeft: false,//如果为flase靠右 为true靠左
       topPos: 0.8,//高度
    });
# 步骤二
<import src="../../template/floatButton/floatButton.wxml" />
<template is="floatButton" data="{{...home}}" />
# 步骤三@import '../../template/floatButton/floatButton.wxss';

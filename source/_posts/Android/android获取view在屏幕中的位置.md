---
layout: post
title: Android 获取view在屏幕中的位置
date: 2020-05-29 22:12:34
tags: 
 - Android
---


**getLocalVisibleRect** ， 返回一个填充的Rect对象， 感觉是这个View的Rect大小，left，top取到的都是0

**getLocalVisibleRect** ， 返回一个填充的Rect对象， 感觉是这个View的Rect大小，left，top取到的都是0
**getGlobalVisibleRect** ， 获取全局坐标系的一个视图区域， 返回一个填充的Rect对象；该Rect是基于总整个屏幕的

**getLocalVisibleRect** ， 返回一个填充的Rect对象， 感觉是这个View的Rect大小，left，top取到的都是0
**getGlobalVisibleRect** ， 获取全局坐标系的一个视图区域， 返回一个填充的Rect对象；该Rect是基于总整个屏幕的
**getLocationOnScreen** ，计算该视图在全局坐标系中的x，y值，（注意这个值是要从屏幕顶端算起，也就是索包括了通知栏的高度）//获取在当前屏幕内的绝对坐标 

**getLocalVisibleRect** ， 返回一个填充的Rect对象， 感觉是这个View的Rect大小，left，top取到的都是0
**getGlobalVisibleRect** ， 获取全局坐标系的一个视图区域， 返回一个填充的Rect对象；该Rect是基于总整个屏幕的
**getLocationOnScreen** ，计算该视图在全局坐标系中的x，y值，（注意这个值是要从屏幕顶端算起，也就是索包括了通知栏的高度）//获取在当前屏幕内的绝对坐标 
**getLocationInWindow** ，计算该视图在它所在的widnow的坐标x，y值，//获取在整个窗口内的绝对坐标 (不是很理解= =、)

**getLocalVisibleRect** ， 返回一个填充的Rect对象， 感觉是这个View的Rect大小，left，top取到的都是0
**getGlobalVisibleRect** ， 获取全局坐标系的一个视图区域， 返回一个填充的Rect对象；该Rect是基于总整个屏幕的
**getLocationOnScreen** ，计算该视图在全局坐标系中的x，y值，（注意这个值是要从屏幕顶端算起，也就是索包括了通知栏的高度）//获取在当前屏幕内的绝对坐标 
**getLocationInWindow** ，计算该视图在它所在的widnow的坐标x，y值，//获取在整个窗口内的绝对坐标 (不是很理解= =、)
**getLeft** , **getTop**, **getBottom**, **getRight**,  这一组是获取相对在它父亲里的坐标

**getLocalVisibleRect** ， 返回一个填充的Rect对象， 感觉是这个View的Rect大小，left，top取到的都是0
**getGlobalVisibleRect** ， 获取全局坐标系的一个视图区域， 返回一个填充的Rect对象；该Rect是基于总整个屏幕的
**getLocationOnScreen** ，计算该视图在全局坐标系中的x，y值，（注意这个值是要从屏幕顶端算起，也就是索包括了通知栏的高度）//获取在当前屏幕内的绝对坐标 
**getLocationInWindow** ，计算该视图在它所在的widnow的坐标x，y值，//获取在整个窗口内的绝对坐标 (不是很理解= =、)
**getLeft** , **getTop**, **getBottom**, **getRight**,  这一组是获取相对在它父亲里的坐标
**注**：如果在Activity的OnCreate()事件输出那些参数，是全为0，要等UI控件都加载完了才能获取到这些

**getLocalVisibleRect** ， 返回一个填充的Rect对象， 感觉是这个View的Rect大小，left，top取到的都是0
**getGlobalVisibleRect** ， 获取全局坐标系的一个视图区域， 返回一个填充的Rect对象；该Rect是基于总整个屏幕的
**getLocationOnScreen** ，计算该视图在全局坐标系中的x，y值，（注意这个值是要从屏幕顶端算起，也就是索包括了通知栏的高度）//获取在当前屏幕内的绝对坐标 
**getLocationInWindow** ，计算该视图在它所在的widnow的坐标x，y值，//获取在整个窗口内的绝对坐标 (不是很理解= =、)
**getLeft** , **getTop**, **getBottom**, **getRight**,  这一组是获取相对在它父亲里的坐标
**注**：如果在Activity的OnCreate()事件输出那些参数，是全为0，要等UI控件都加载完了才能获取到这些
**example:**

 int[] location = new int[2];    v.getLocationOnScreen(location); 

 int x = location[0]; 

 int y = location[1];
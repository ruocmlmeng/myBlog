---
title: Android
date: 2023-11-15 20:27:13
tags:
  - Android
category: Android
top_img: /images/backgroundFriend.png
cover: /images/backgroundFriend.png
ai:
  - 本教程介绍Android的基本知识
  - 本文真不错
---
# Android_oneDay

## 1.运行日志

<img alt="" src="./Android/android.png"/>

## 2.设置文本大小

>- 在Java代码中调用setTextSize方法，即可指定文本大小。
>
>- 在XML文件中则通过属性android:textsize指定文本大小，此时需要指定字号单位。
>
>pX：它是手机屏幕的最小显示单位，与设备的显示屏有关。
>dp：它是与设备无关的显示单位，只与屏幕的尺寸有关。
>Sp：它专门用来设置字体大小，在系统设置中可以调整字体大小。

## 3.TextView-基础文本

### 3.1基础属性详解

> 1.layout_width：组件的宽度
>
> 2.layout_height：组件的高度
>
> 3.id：为TextView设置一个组件ic
>
> 4.text：设置显示的文本内容
>
> 5.textColor：设置字体颜色
>
> 6.textStyle：设置字体风格，三个可选值：normal(无效果），bold(加粗），italic(体）
>
> 7.textSize：字体大小，单位一般是用sp
>
> 8.background：控件的背景颜色，可以理解为填充整个控件的颜色，可以是图片
>
> 9.gravity：设置控件中内容的对齐方向，TextView中是文字，ImageView中是图片等等。

### 3.2.带阴影的TextView

> 1.android:shadowColor:设直阴影颜色，需要与shadowRadius一起使用
>
> 2.android:shadowRadiug:设置阴影的模糊程度设为0.1就变成字体颜色了，建议使用3.0
>
> 3.android:shadowDx:设置阴影在水平方向的偏移,就是水平方向阴影开始的横坐标位置
>
> 4.android:shadowDy:设置阴影在竖直方向的偏移就是竖直方向阴影开始的纵坐标位置

### 3.3.实现跑马灯效果的TextView

> 1.android:singleLine:内容单行显示
>
> 2.android：focusable：是否可以获取焦点
>
> 3.androidfocusablelnTouchMode：用于控制视图在触摸模式下是否可以聚焦
>
> 4.android:ellipsize:在哪里省略文本
>
> 5.android:marqueeRepeatLimit：字幕动画重复的次数

## 6.EditText-编辑文本

### 6.1主要属性

> 1.android:hint输入提示
>
> 2.android:textColorHint输入提示文字的颜色
>
> 3.android:inputType输入类型
>
> 4.android:drawableXxxx在输入框的指定方位添加图片
>
> 5.android:drawablePadding设置图片与输入内容的间距
>
> 6.android:paddingXxxx设置内容与边框的间距
>
> 7.android:background背景色

## 7.ImageView-图片的放缩

### 7.1主要属性

> 1.android:src设置图片资源
>
> 2.android:scaleType设置图片缩放类型
>
> 3.android:maxHeight最大高度
>
> 4.android:maxWidth最大宽度
>
> 5.android:adjustViewBounds调整View的界限

### 7.2缩放类型

> 1.fitStart保持宽高比缩放图片，直到较长的边与Image的边长相等，缩放完成后将图片放在ImageView的左上
>
> 2.fitCenter默认值，同上，缩放后放于中间
>
> 3.fitEnd同上，缩放后放于右下角
>
> 4．fitxY对图像的横纵方向进行独立缩放，使得该图片完全适应ImageView，但是图片的宽高比可能会发生改
>
> 5.center保持原图的大小，显示在ImageView的中心。当原图的size大于ImageView的size，超过部分裁剪处理
>
> 6.centerCrop保持宽高比缩放图片，直到完全覆盖ImageView，可能会出现图片的显示不完全
>
> 7.centerlnside保持宽高比缩放图片，直到ImageView能够完全地显示图片
>
> 8.matrix不改变原图的大小，从ImageView的左上角开始绘制原图，原图超过ImageView的部分作裁剪处理

## 8.ProgressBar-进度条

### 8.1常用属性详解

> 1.android:max：进度条的最大值
>
> 2.android:progress：进度条已完成进度值
>
> 3.android:indeterminate：如果设置成true，则进度条不精确显示进度
>
> 4.style="?android:attr/progressBarStyleHorizontal"水平进度条

## 9.Toolbar

### 9.1主要属性

> android:layout width="matchparent"
>
> android:layoutheight-"?attr/actionBarSize"
>
> android:background="#ffffoo"
>
> app:navigationlcon="@drawable/ic_baseline_arrow_back_24"
>
> app:title="主标题"
>
> app:titleTextColor="#ffoooo"
>
> app:titleMarginStart="90dp"
>
> app:subtitle="子标题"
>
> I
>
> app:subtitleTextColor="#ooffff"
>
> app:logo="@mipmap/iclauncher


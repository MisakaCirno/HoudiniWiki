---
title: 操作 - 参数面板
author: 御琪幽然
description: 
date: 2022-10-08
pan: 
video: 
weight: 1
slug: 9b5d7fdc
version: Houdini 19+
producer: 
level: 
tags: 
  - 
nodes:
  - 
pipeline:
  - 
---

# 一、简介
显示节点参数的面板。

# 二、操作&快捷键

## 切换
-   Alt+3（小键盘3）：切换当前区域显示为Parameters。

## 操作
-   在任何需要输入数值的编辑框中，按下鼠标中键都可以打开滑动调整工具。对于有多个值的参数，在参数名称上点击中键可以同时调整所有值的大小。
-   点击参数名可以切换引用路径的代码和数值的显示，或者相对路径与绝对路径的显示等。
-   Ctrl+中键点击参数的名称，可以将该参数重置为默认值。
-   Alt+左键点击参数的值，可为该值添加关键帧。
-   Shift+左键/中键点击参数的值，可以打开曲线编辑器窗口。
-   Ctrl+Shift+左键点击参数的名称，可以将参数的引用关系清除。
-   在一个参数框中右键，选择Copy Parameter，然后再另一个参数框中右键，选择Paste Relative References，可以将前者引用至后者处，当前被引用参数改变时，引用参数也会随之改变。
粘贴的结构类似于`ch("../leg_height/scale")`，“ch”代表channel的意思，括号中则是参数的整体路径。

-   点击节点名称右侧的齿轮，选择Edit Parameter Interface，可以打开该节点的参数编辑面板。
在该面板中，可以为当前节点添加各类的参数。
参数有一个Name，有一个Label，前者用于互相调用，后者用于在参数面板中显示。

# 三、其他
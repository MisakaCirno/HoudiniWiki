---

title: Entagma Patreon - Vex 101
author: 智伤帝
description: Entagma VEX 入门课程
date: 2021-02-19
pan: https://pan.baidu.com/s/1epLzq4F2c9uTsYZBZ92QWg
video: https://www.bilibili.com/video/BV1g7411q7BQ
weight: 3
slug: 554149d6
version: houdini 16+
producer: Entagma
level: beginner
tags: 
  - VEX
nodes:
  - SOP
pipeline:
  - modeling

---

## 总结


## 观看笔记

![02](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/01.jpg)

> &emsp;&emsp;wrangle 节点可以设置为 Number 类型自定义执行的次数。

---

09 - chladni pattern

[克拉尼图形](https://baike.baidu.com/item/%E5%85%8B%E6%8B%89%E5%B0%BC%E5%9B%BE%E5%BD%A2)

> &emsp;&emsp;克拉尼图形 - 声音可视化

https://thelig.ht/chladni/

```
s(x, y) = asin(πnx) sin(πmy) + bsin(πmx)sin(πny)
```

> &emsp;&emsp;克拉尼图形 算法

![09](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/02.jpg)

> &emsp;&emsp;Houdini16 之后内置 PI 变量，更老的版本需要手动添加 PI 

![09](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_03.jpg)

> &emsp;&emsp;使用公式写 VEX 代码比用 Vop 节点复现公式代码来得方便。

---

> &emsp;&emsp;Mortiz 推荐 Joy of Vex 出自 CGwiki 的系列文章教程作为额外的学习材料 [链接](https://www.tokeru.com/cgwiki/index.php?title=JoyOfVex)

![14](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/03.jpg)

> &emsp;&emsp;Vex 可以通过 include 将预制的函数引入。

![14](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/04.jpg)

> &emsp;&emsp;需要在 Houdini.env 里面引入文件目录。

---

![15](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/05.jpg)

> &emsp;&emsp;Houdini 的 foreach 和 compile 都比 wrangle 节点要慢很多。


## 案例分析

### 法线朝向

<video src="https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_01.mp4" autoplay loop muted width=100%></video>

{{<attachments pattern="example_01.hip" />}}

### 噪波面片

<video src="https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_02.mp4" autoplay loop muted width=100%></video>

{{<attachments pattern="example_02.hip" />}}

### chladni pattern 克拉尼图形

![09](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_03.jpg)

![09](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_03_01.jpg)

{{<attachments pattern="example_03.hip" />}}

### sin cos 变化线圈

![10](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_04.jpg)

> &emsp;&emsp;sin 结合 cos 可以构成一个圆圈。
> &emsp;&emsp;加上 frequency 参数动态变化 sin 和 cos 的参数值就可以得到上面效果的线段。
> &emsp;&emsp;再使用 polywire 生成几何体。

{{<attachments pattern="example_04.hip" />}}

### 临近点线段

![11](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_05.jpg)

> &emsp;&emsp;这个效果参考 Vex Fundamentals 教程 [链接](/zh/dbcc6763/#寻找临近的点生成线---16)

![12](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_06.jpg)

{{<attachments pattern="example_06.hip" />}}

### 多重切分

![13](https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_07.jpg)

{{<attachments pattern="example_07.hip" />}}

### Catenary 算法

<video src="https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_08.mp4" autoplay loop muted width=100%></video>

{{<attachments pattern="example_08.hip" />}}

### 交错线碰撞

<video src="https://cdn.jsdelivr.net/gh/FXTD-ODYSSEY/HoudiniWiki@gh-pages/posts/554149d6/example_09.mp4" autoplay loop muted width=100%></video>

> &emsp;&emsp;wrangle 可以根据组去遍历相关的顶点。

{{<attachments pattern="example_09.hip" />}}



what do you think your new keyboard
i still not very get used to it 
but right now, it almost fine at that moment.

我尝试打些中文，试试我的新键盘，感觉非常良好。
打字还很安静，不会有噼里啪啦的敲键盘声音。

而且这个键盘还是蓝牙键盘，可以无线远程连接。
总体感觉稍微适应一下，感觉非常良好~
终于摆脱了以前的垃圾旧键盘的使用了_(:з」∠)_。
























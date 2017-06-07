# 实验四、滚动相册

### 实验背景

在网页中一个固定位置，通过滚动方式显示更多信息，一个是节省了网页空间，第二，让网页整体效果看起来更灵活，更吸引人，很多网站通过循环滚动图片或循环滚动文字的方式展示更多的信息，这个功能是如何实现的呢？

### 实验目的
- 掌握图片滚动的原理
- 掌握函数 setInterval() 和 clearInterval() 的使用；
- 掌握属性 scrollLife 和 offsetWidth 的用法；

### 实验步骤
**步骤一：搭建 HTML 结构和 CSS 样式**

- 文件目录结构；
- 创建 HTML 结构；
- 设计 CSS 样式，必须为包围图片的 div 设置属性；

**步骤二：让图片向左移动一点（比如向左移动 1px）**

- 自定义一个函数 changeToLeft，该函数的功能，实现图片的向左移动；
- 在函数 changeToLeft 里，使用属性 scrollLeft 设置元素的滚动条的水平偏移值；

**步骤三：让图片每隔 10 毫秒就向左移动 1px**

- 使用函数 setinterval()，每隔10毫秒调用一次函数 changeToLeft
- 所有图片滚动到左侧边缘后，就停止滚动了，为什么？

**步骤四：让图片循环滚动**

- 将 id 为 picScroll2 的元素里的代码设置为和 picScroll1 里的代码完全一致；
- 最外层 div 向左偏移值大于 picScroll1 的宽度时，重新设置最外层 div 的左偏移值为 0，否则继续向左滚动；

提示：获取 picScroll1 的宽度，课通过对象的 offsetWidth 属性得到。

**步骤五：添加事件，鼠标经过时，图片停止滚动**

- 为最外层 div 添加事件 onmouseover。
- 触发事件 onmouseover 时，使用函数 clearInterval()，取消函数 setInterval() 函数的执行；

**步骤六：添加事件：鼠标离开时，图片继续滚动**
- 为最外层 div 添加事件 onmouseout。
- 触发事件 onmouseout 时，开始图片向左滚动的执行；
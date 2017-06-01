# 实验二、简单计算器

运用已掌握的知识，做一个能实现简单功能的计算器。

### 实验步骤

##### 步骤一：HTML 设计页面结构

用表格和按钮完成，每个按钮设置 value 属性，给结果框设置 id 属性。

##### 步骤二：为页面的 HTML 代码应用 CSS 进行修饰

结果框中的内容是从右向左显示的。

##### 步骤三：编写外部 JavaScript 文件

1. 用户输入的值存入全局变量，因为有多个函数会用到

2. 书写数据显示函数 showData()。将用户点击过的数据显示出来，主要语句是：document.getElementById("result").innerHTML = str;

3. 将运算结果显示到结果框中，用一个函数 calculate() 完成。具体分为三步，第一步是当用户点击等号是，结果框中清除原有内容，用 document.getElementById("result").innerHTML='';第二步是进行计算，可以用eval()函数来完成，计算某个字符串，并返回计算结果，可以将结果存在resultNum，仍然是使用：document.getElementById("result").innerHTML = resultNum；第三步是将结果显示在结果框中。

4. 当用户点击 C 时，字符串被清空，并将结果框的内容清为零。可以用函数clearData()来完成。

5. 编写事件响应函数，并添加到 HTML 元素上。

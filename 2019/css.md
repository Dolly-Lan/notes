### BEM命名规范

[官网](http://getbem.com/introduction/)

B = Block = 块：UI框架中可以重复使用的组件，具有唯一性的命名，相当于声明了一个独立的命名空间。如 ：Tabs、Form、Menu

E = Element = 元素：Block的子元素且和Block语义相关。如：Menu item、List item

M = Modifier = 修饰符：用于修饰Block或Element，标识外观和行为。如：active、red

BEM规范就是以如下方式来指定样式名称：

“__”下划线连接“块”和“元素

“--”双连字符用于修饰“块”或“元素”

备注： “-”单连字符可以用于连接B、E、M中不同的单词，如：menu-header__item--active


### 连续英文、标点符号自动换行

      word-break: normal;
      word-wrap:break-word;

### 表格内强制断行

step1:

      table{
        width: 100%; // 给出宽度
        table-layout: fixed;
      }
      
step2: colgroup指定列宽

      <colgroup>
            <col width="14%"></col>
            <col width="2%"></col>
            <col width="84%"></col>
      </colgroup>
      
step3:

      tr{
          word-wrap:break-word;
      }

### :not(selector)

      button:not([disabled]) { background: red; }  //表示属性为disabled的button标签背景色为红色

### transform以中心缩放平移

https://segmentfault.com/a/1190000009248258

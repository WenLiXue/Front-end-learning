# HTML笔记
## 介绍
    HTML: HyperText Markup Language 超文本标记语言
### 标签
    标签分类：单标签 双标签
    例子：单标签：<标签名>
    双标签：<标签名> </标签名>
### 元素
    分类：包括行内元素和块内元素
    行内元素：<input> <span>等  特点：元素不独占一行 一行有多个
    块内元素:<p> <div>等        特点：元素独占一行，一行只有一个
    块内元素和行内元素的规则：
    <!-- 规则1：块级元素能写：行内元素、块级元素-->
    <!-- 规则2：行内元素只能写行内元素不能写块级元素-->
### 文本标签
```html
<!--常用文本标签-->
<em> 这个是斜体</em>   
<strong>这个是加粗</strong>
<span>这个是普通文本标签</span>
<!--不常用文本标签-->
```
### 图片标签
    格式如下
```html
<img src="" alt="" width="">
```
    属性含义：
    src：表示的是图片的地址
    alt:表示的是图片的描述  搜索引擎会搜索到
    width：表示的是图片的宽度设置，高度不用设置，等比例缩放
### 超文本标签
    格式如下：
```html
<a href="" target=""></a>
```
    属性含义：
    href:表示的是要跳转的网页网址
    target：表示跳转的方式  _blank表示新标签页  _self表示原标签页
### 锚点

### 列表
    分类：
    有序列表，ordered list <ol>
    无序列表，unodered list <ul>
    自定义列表 definition list <dl>

### 表格
    表格的组成:标题 头部 主体 注脚
```html
     <table border="1">
    <!--        表格标题-->
    <caption>学生信息</caption>
    <!--        表格头部-->
    <thead>
    <tr>
        <th>姓名</th>
        <th>性别</th>
        <th>年龄</th>
        <th>民族</th>
        <th>政治面貌</th>
    </tr>
    </thead>
    <!--    表格主体-->
    <tbody>
    <tr>
        <td>张三</td>
        <td>男</td>
        <td>18</td>
        <td>汉族</td>
        <td>团员</td>
    </tr>
    <tr>
        <td>李四</td>
        <td>男</td>
        <td>18</td>
        <td>满族</td>
        <td>群众</td>
    </tr>
    <tr>
        <td>王五</td>
        <td>女</td>
        <td>20</td>
        <td>汉族</td>
        <td>团员</td>
    </tr>
    <tr>
        <td>赵六</td>
        <td>男</td>
        <td>42</td>
        <td>汉族</td>
        <td>党员</td>
    </tr>
    </tbody>

    <!--        表格脚注-->
    <tfoot>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>共计：4人</td>
    </tfoot>
</table>
```
    几个标签的解释：
    <th> 是表格头部单元格的标签
    <td> 是表格非头部单元格的标签
    <tr> 表示的是表格的一行
### 常用标签补充
    <br> 换行标签
    <hr> 分割线标签
    <pre>表示按原文显示（一般用于在页面中嵌入一大段代码）
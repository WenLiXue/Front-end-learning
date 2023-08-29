# CSS学习
## CSS的语法
css语法包括两个部分一个是选择器一个是属性（一条或多条声明）
```html

<style>
    h1
    {
        color:red;
        font-size:20px;
    }
</style>
```
## CSS引入的三种方式
* 第一种:
    ```html
        <p style="color: red;font-size: 20px">这个是内联样式的方案</p>
    ```
* 第二种
    ```html
    <head>
        <meta charset="UTF-8">
        <title>CSS引入方式</title>
    <!-- 内部样式方案-->
        <style>
            p{
                color: red;
                font-size: 30px;
            }
        </style>
    </head>
    <body>
        <p>内部样式表</p>
    </body>
    ```
* 第三种  在head中引入已经编写好的css文件
    ```html
    <head>
        <meta charset="UTF-8">
        <title>css外部引入</title>
        <link rel="stylesheet" href="../CSS外部样式/public.css">
    </head>
    <body>
        <p>
            This is a test
        </p>
        <a href="../../HTML5.html"> 转到HTML5网页</a>
    </body>
    </html>
    ```
## CSS选择器
* 全局选择器 :所有的标签都被选择 统一样式
    ```html
    <!--全局选择器为任何选择器统一样式  用作通配符-->
    <style>
        *{
            color: red;
            font-size: 30px;
        }
    </style>
    ```
*  元素选择器
    ```html
    <head>
        <meta charset="UTF-8">
        <title>元素选择器</title>
    <!--    让所有的指定标签全部统一-->
        <style>
            span{
                color: green;
            }
        </style>
    </head>
    <body>
        <p>1</p>
        <p>1</p>
        <p>1</p>
        <p>1</p>
        <p>1</p>
        <p>1</p>
        <p>123！ <span>芜湖</span></p>
    </body>
    ```
* 类选择器
    ```html
    <head>
        <meta charset="UTF-8">
        <title>类选择器</title>
        <style>
            .content{
                color: red;
            }
            .size{
                color: blue;
                font-size: 30px;
            }
        </style>
    </head>
    <body>
    <!--class可以重复使用-->
        <p class="size">大家好</p>
        <p>你们好</p>
        <p class="content">我不好！</p>
        <p class="content">我哭了！</p>
        <div class="content">这是个div</div>
    </body>
    ```
* ID选择器
    ```html
    <head>
        <meta charset="UTF-8">
        <title>ID选择器</title>
        <style>
            #mytitle{
                color: red;
                font-size: 40px;
            }
        </style>
    </head>
    <body>
    <!-- id 不能重复 重复了会报错-->
        <p id="mytitle">HELLO!</p>
    </body>
    ```
* 合并选择器
    ```html
    <head>
        <meta charset="UTF-8">
        <title>合并选择器</title>
        <style>
            p,div{
                color: red;
            }
            .test,.good{
                color: blue;
                font-size: large;
            }
        </style>
    </head>
    <body>
        <p>这是p标签</p>
        <div>这个是div标签</div>
        <span class="test">这是一个span标签</span>
        <li class="good">这是一个li标签</li>
    </body>
    ```
### 选择器的优先级：
    行内样式 1000>ID选择器 100>类选择器 10>元素选择器 1

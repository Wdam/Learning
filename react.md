# react

## hello_react

jsx语法

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>hello react</title>
</head>
<body>
    <div id="test"></div>

    <script src="https://unpkg.com/react@17/umd/react.development.js" crossorigin></script>
    <script src="https://unpkg.com/react-dom@17/umd/react-dom.development.js" crossorigin></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    
    <script type="text/babel">
        //创建虚拟dom
        const VDOM = <h1>hello react </h1>
        //渲染虚拟dom到页面
        ReactDOM.render(VDOM,document.getElementById('test'))
    </script>

</body>
</html>
~~~

js语法

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>hello react</title>
</head>
<body>
    <div id="title"></div>

    <script src="https://unpkg.com/react@17/umd/react.development.js" crossorigin></script>
    <script src="https://unpkg.com/react-dom@17/umd/react-dom.development.js" crossorigin></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

    <script type="text/javascript">
        const VDOM = React.createElement('h1',{id:'title'},'hello react jsx')
        ReactDOM.render(VDOM,document.getElementById('title'))
    </script>
~~~

### jsx语法规则

全称：JavaScript XML

react定义的一种类似于xml的js扩展语法

作用：用来简化创建虚拟dom

1. 写法：var ele = ` <h1>hello jsx</h1>`
2. 他不是字符串也不是html/xml标签
3. 他最终产生就是一个js对象

标签名任意


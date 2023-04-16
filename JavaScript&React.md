<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

  - [条件运算符](#%E6%9D%A1%E4%BB%B6%E8%BF%90%E7%AE%97%E7%AC%A6)
  - [typeof 操作符](#typeof-%E6%93%8D%E4%BD%9C%E7%AC%A6)
  - [**constructor** 属性](#constructor-%E5%B1%9E%E6%80%A7)
  - [错误](#%E9%94%99%E8%AF%AF)
  - [console.log() 方法](#consolelog-%E6%96%B9%E6%B3%95)
  - [严格模式(use strict)](#%E4%B8%A5%E6%A0%BC%E6%A8%A1%E5%BC%8Fuse-strict)
  - [===](#)
  - [使用误区](#%E4%BD%BF%E7%94%A8%E8%AF%AF%E5%8C%BA)
  - [Undefined 不是 Null](#undefined-%E4%B8%8D%E6%98%AF-null)
  - [this 关键字](#this-%E5%85%B3%E9%94%AE%E5%AD%97)
  - [let 和 const](#let-%E5%92%8C-const)
  - [**javascript****:void(0)**](#javascriptvoid0)
  - [href="#"](#href)
  - [JavaScript 异步编程](#javascript-%E5%BC%82%E6%AD%A5%E7%BC%96%E7%A8%8B)
  - [Promise](#promise)
  - [箭头函数](#%E7%AE%AD%E5%A4%B4%E5%87%BD%E6%95%B0)
  - [类](#%E7%B1%BB)
    - [继承](#%E7%BB%A7%E6%89%BF)
    - [静态方法](#%E9%9D%99%E6%80%81%E6%96%B9%E6%B3%95)
- [Nodejs](#nodejs)
  - [引入模块](#%E5%BC%95%E5%85%A5%E6%A8%A1%E5%9D%97)
- [React](#react)
  - [函数组件和类组件](#%E5%87%BD%E6%95%B0%E7%BB%84%E4%BB%B6%E5%92%8C%E7%B1%BB%E7%BB%84%E4%BB%B6)
  - [JSX](#jsx)
  - [State Hook](#state-hook)
  - [*Effect Hook*](#effect-hook)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## 条件运算符

```Bash
variablename=(condition)?value1:value2 
```

## typeof 操作符

```Bash
typeof "John"                // 返回 string
typeof 3.14                  // 返回 number
typeof false                 // 返回 boolean
typeof [1,2,3,4]             // 返回 object
typeof {name:'John', age:34} // 返回 object
```

##  **constructor** 属性

返回所有 JavaScript 变量的构造函数。

```Bash
"John".constructor                 // 返回函数 String()  { [native code] }
(3.14).constructor                 // 返回函数 Number()  { [native code] }
false.constructor                  // 返回函数 Boolean() { [native code] }
[1,2,3,4].constructor              // 返回函数 Array()   { [native code] }
{name:'John', age:34}.constructor  // 返回函数 Object()  { [native code] }
new Date().constructor             // 返回函数 Date()    { [native code] }
function () {}.constructor         // 返回函数 Function(){ [native code] }
```

## 错误

```Bash
try {
    ...    //异常的抛出
} catch(e) {
    ...    //异常的捕获与处理
} finally {
    ...    //结束处理
}
```

##  console.log() 方法

```Bash
console.log(c);
```

## 严格模式(use strict)

严格模式下你不能使用未声明的变量,"use strict" 必须至于顶行

```Bash
<script>
    "use strict";
    x = 3.14;       // 报错 (x 未定义)
</script>
```

## ===

在严格的比较运算中，=== 为恒等计算符，同时检查表达式的值与类型，以下 if 条件语句返回 false：

## 使用误区

https://www.runoob.com/js/js-mistakes.html

## Undefined 不是 Null

## this 关键字

```JavaScript
var person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};
```

可以显示绑定

```JavaScript
var person1 = {
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
}
var person2 = {
  firstName:"John",
  lastName: "Doe",
}
person1.fullName.call(person2);  // 返回 "John Doe"
```

##  let 和 const

const 声明一个只读的常量，一旦声明，常量的值就不能改变。

let 声明的变量只在 let 命令所在的代码块 **{}** 内有效，在 **{}** 之外不能访问。

```JavaScript
var x = 10;
// 这里输出 x 为 10
{ 
    var x = 2;
    // 这里输出 x 为 2
}
// 这里输出 x 为 2

var x = 10;
// 这里输出 x 为 10
{ 
    let x = 2;
    // 这里输出 x 为 2
}
// 这里输出 x 为 10
```

## **javascript****:void(0)**

**void** 是 JavaScript 中非常重要的关键字，该操作符指定要计算一个表达式但是不返回值。

```JavaScript
<a href="javascript:void(0)">单击此处什么也不会发生</a>
```

## href="#"

在页面很长的时候会使用 **#** 来定位页面的具体位置，格式为：**# + id**。

```JavaScript
<a href="javascript:void(0);">点我没有反应的!</a>
<a href="#pos">点我定位到指定位置!</a>
<br>
...
<br>
<p id="pos">尾部定位点</p>
```

## JavaScript 异步编程

```JavaScript
setTimeout(function () {
    document.getElementById("demo1").innerHTML="RUNOOB-1!";
}, 3000);

$.get("https://www.runoob.com/try/ajax/demo_test.php",function(data,status){
    alert("数据: " + data + "\n状态: " + status);
});
```

## Promise

新建一个promise对象

```JavaScript
new Promise(function (resolve, reject) {
    // 要做的事情...
})
```

例子

```JavaScript
function print(delay, message) {
    return new Promise(function (resolve, reject) {
        setTimeout(function () {
            console.log(message);
            resolve();
        }, delay);
    });
}

print(1000, "First").then(function () {
    return print(4000, "Second");
}).then(function () {
    print(3000, "Third");
});

async function asyncFunc() {
    await print(1000, "First");
    await print(4000, "Second");
    await print(3000, "Third");
}
asyncFunc();
```

## 箭头函数

箭头函数表达式的语法比普通函数表达式更简洁。

```JavaScript
// (参数1, 参数2, …, 参数N) => { 函数声明 }
// (参数1, 参数2, …, 参数N) => 表达式(单一)

const x = (x, y) => x * y; // 如果函数部分只是一个语句，则可以省略 return 关键字和大括号 {}，这样做是一个比较好的习惯:

const materials = [
  'Hydrogen',
  'Helium',
  'Lithium',
  'Beryllium'
];

console.log(materials.map(material => material.length));
```

## 类

每个类中包含了一个特殊的方法 **constructor()**，它是类的构造函数，这种方法用于创建和初始化一个由 **class** 创建的对象。

```JavaScript
class Stonebird {
  constructor(name, url) {
    this.name = name;
    this.url = url;
  }
}
```

### 继承

```JavaScript
class Site {
  constructor(name) {
    this.sitename = name;
  }
  present() {
    return '我喜欢' + this.sitename;
  }
}
 
class Runoob extends Site {
  constructor(name, age) {
    super(name);
    this.age = age;
  }
  show() {
    return this.present() + ', 它创建了 ' + this.age + ' 年。';
  }
}
 
let noob = new Runoob("菜鸟教程", 5);
document.getElementById("demo").innerHTML = noob.show();
```

### 静态方法

静态方法是使用 static 关键字修饰的方法，又叫类方法，属于类的，但不属于对象，在实例化对象之前可以通过 **类名.方法名** 调用静态方法。静态方法不能在对象上调用，只能在类中调用

```JavaScript
class Runoob {
  constructor(name) {
    this.name = name;
  }
  static hello() {
    return "Hello!!";
  }
}
 
let noob = new Runoob("菜鸟教程");
 
// 可以在类中调用 'hello()' 方法
document.getElementById("demo").innerHTML = Runoob.hello();
```

# Nodejs

## 引入模块

我们使用 **require** 指令来载入 http 模块

```JavaScript
var http = require("http");
```

# React

## 函数组件和类组件

## JSX

## State Hook

```JavaScript
import React, { useState } from 'react';

function Example() {
  // 声明一个叫 "count" 的 state 变量
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

等价的class

```JavaScript
class Example extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }

  render() {
    return (
      <div>
        <p>You clicked {this.state.count} times</p>
        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
          Click me
        </button>
      </div>
    );
  }
}
```

## *Effect Hook* 

*Effect Hook* 可以让你在函数组件中执行副作用操作

```JavaScript
import React, { useState, useEffect } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  // Similar to componentDidMount and componentDidUpdate:
  useEffect(() => {
    // Update the document title using the browser API
    document.title = `You clicked ${count} times`;
  });

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```
# JavaScript Manual

## Table of Contents
- Basic
  - [Introduction](#introduction)
  - [Editor for JavaScript](#editor-for-javascript)
  - [Using JavaScript](#using-javascript)
  - [Console Log](#console-log)
  - [Variables](#variables)
  - [Const/Let](#const-let)
  - [Data Types in JavaScript](#data-types-in-javascript)
  - [Type Conversion](#type-conversion)
  - [Operators](#operators)
  - [Math](#math)
  - [String Method](#string-method)
    - [indexOf](#index-of)
    - [lastIndexOf](#last-index-of)
    - [concat](#concat)
  - [Template Strings](#template-strings)
  - [Array Helper Methods](#array-helper-methods)
    - [join](#join)
    - [push](#push)
    - [pop](#pop)
    - [shift](#shift)
    - [unshift](#unshift)
    - [splice](#splice)
    - [slice](#slice)
    - [split](#split)
    - [forEach](#foreach)
    - [map](#map)
    - [filter](#filter)
    - [find](#find)
    - [findIndex](#find-index)
    - [every and some](#every-and-some)
    - [reduce](#reduce)
    - [sort](#sort)
  - Strict Mode
  - Dynamic Typing
  - Hoisting
  - Functions
    - Creating and Calling Them
    - Arguments & Returning Data
  - Control Structures
    - If statement
    - Switch & Break
    - For Loop
    - Nested Loops
    - controlling Loops with break & continue
    - For Loop varintions
    - Looping through Arrays
    - While Loop
  - Types & Scope
    - Primitive vs Reference Types
    - Global vs Local Scope
  - [Arrow Function](#arrow-function)
  - [Enhanced Object Literals](#enhanced-object-literals)
  - [Default Function Argument](#default-function-argument)
  - Rest and Spread Operator
    - [Rest and Spread](#capturing-arguments)
  - [Destructuring](#destructuring)
  - [Classed](#classes)
    - [Introduction](#introduction)
    - [Prototypal Inheritance](#prototypal-inheritance)
    - [Refactoring with Classes](#refactoring-with-classes)
  - ทบทวนเรื่องออบเจ็กต์
    - this
    - [call() apply() และ bind()](#call-apply-bind)
  - ทบทวนเรื่องการแสดงความผิดพลาด Error
- Intermediate
  - [Callback](#callback)
    - [Recursive Function](#recursive-function)
  - [Promise](#promise)
  - Event loop
  - [Reactive](#reactive)
  - Testing
    - Reference
      - [Mocha](https://mochajs.org/)
      - [Expect](https://github.com/mjackson/expect)
      - [Super Test](https://github.com/visionmedia/supertest)
      - [Chai](http://chaijs.com/)
      - [Jest](https://facebook.github.io/jest/)
- Advance
- Learning More
  - Lodash
  - Moment
  - Axios
  - RxJS
  - React
  - React-Native
  - Vue
  - Angular
  - Webpack
  - TypeScript
  - Meteor
  - Electron
  - GraphQL
  - Elixir
  - Next.JS
- Reference
  - [Airbnb JavaScript Style Guide](#airbnb)
  - [JavaScript Standard Style](#standard)
  - [ES2015+ cheatsheet](https://devhints.io/es6)
- Blog
  - [แปลและสรุปเรื่อง Ten Things A *Serious* JavaScript Developer Should Learn by somkiat.cc](http://www.somkiat.cc/summary-10-things-a-serious-javascript-developer-should-learn/)
  - [การใช้งาน array พื้นฐาน by CamPus](https://medium.com/@camp191/javascript-%E0%B8%88%E0%B8%B1%E0%B8%94%E0%B8%81%E0%B8%B2%E0%B8%A3-array-%E0%B9%81%E0%B8%9A%E0%B8%9A%E0%B8%87%E0%B9%88%E0%B8%B2%E0%B8%A2%E0%B9%86-%E0%B8%94%E0%B9%89%E0%B8%A7%E0%B8%A2-map-filter-reduce-%E0%B9%81%E0%B8%A5%E0%B8%B0%E0%B8%9C%E0%B8%AD%E0%B8%87%E0%B9%80%E0%B8%9E%E0%B8%B7%E0%B9%88%E0%B8%AD%E0%B8%99-bfc84e59ebae)
  - [ความรู้สึกเมื่ออยากเขียน JavaScript ในปี 2016](https://medium.com/@noomerzx/%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B8%A3%E0%B8%B9%E0%B9%89%E0%B8%AA%E0%B8%B6%E0%B8%81%E0%B9%80%E0%B8%A1%E0%B8%B7%E0%B9%88%E0%B8%AD%E0%B8%AD%E0%B8%A2%E0%B8%B2%E0%B8%81%E0%B9%80%E0%B8%82%E0%B8%B5%E0%B8%A2%E0%B8%99-javascript-%E0%B9%83%E0%B8%99%E0%B8%9B%E0%B8%B5-2016-92711cf3987)
  - [javascript 101 by noomerZx](https://stories.sellsuki.co.th/js-101-%E0%B8%9E%E0%B8%B7%E0%B9%89%E0%B8%99%E0%B8%90%E0%B8%B2%E0%B8%99%E0%B8%97%E0%B8%B5%E0%B9%88-%E0%B8%95%E0%B9%89%E0%B8%AD%E0%B8%87%E0%B8%AB%E0%B9%89%E0%B8%B2%E0%B8%A1-%E0%B8%9E%E0%B8%A5%E0%B8%B2%E0%B8%94-bac5de6f9900)
  - [javascript 102 by noomerZx](https://stories.sellsuki.co.th/js-102-%E0%B8%9E%E0%B8%B7%E0%B9%89%E0%B8%99%E0%B8%90%E0%B8%B2%E0%B8%99-javascript-%E0%B8%97%E0%B8%B5%E0%B9%88-%E0%B8%84%E0%B8%B8%E0%B8%93-%E0%B8%AD%E0%B8%B2%E0%B8%88%E0%B9%84%E0%B8%A1%E0%B9%88%E0%B9%80%E0%B8%84%E0%B8%A2%E0%B8%A3%E0%B8%B9%E0%B9%89-19e87fc6b452)
  - [javascript 103 by noomerZx](https://stories.sellsuki.co.th/js-103-%E0%B8%9E%E0%B8%B7%E0%B9%89%E0%B8%99%E0%B8%90%E0%B8%B2%E0%B8%99-javascript-%E0%B8%97%E0%B8%B5%E0%B9%88-%E0%B8%A5%E0%B8%B6%E0%B8%81-%E0%B8%8B%E0%B8%B6%E0%B9%89%E0%B8%87-832de08f824)
- E-Learning
  - [The Coding Interview Bootcamp: Algorithms + Data Structure](https://www.udemy.com/coding-interview-bootcamp-algorithms-and-data-structure)
  - [ES6 Javascript: The Complete Developer's Guide](https://www.udemy.com/javascript-es6-tutorial/)
  - [Accelerated JavaScript Training](https://www.udemy.com/javascript-bootcamp-2016)
  - [Accelerated ES6 JavaScript Training](https://www.udemy.com/es6-bootcamp-next-generation-javascript)
  - [Beginner's ES6 Programming. Code for the Web in JavaScript](https://www.udemy.com/beginners-es6-programming-code-for-the-web-in-javascript)
  - [ฟรี! เตรียมพื้นฐาน ES2015 และ Node.js ก่อนไปลุย React](https://www.skilllane.com/courses/basic-es2015-nodejs-before-react)
  - [ฟรี! Javascript คืออะไร - วีดีโอสอน Javascript](https://www.youtube.com/watch?v=BAG5BP5exmA&list=PL9uXbYsezM7mkf4w5tmillxVq9fHyslwT&index=1)
- Book
  - [หนังสือ พัฒนาเว็บแอปพลิเคชั่นด้วย JavaScript](https://www.se-ed.com/product/%E0%B8%9E%E0%B8%B1%E0%B8%92%E0%B8%99%E0%B8%B2%E0%B9%80%E0%B8%A7%E0%B9%87%E0%B8%9A%E0%B9%81%E0%B8%AD%E0%B8%9B%E0%B8%9E%E0%B8%A5%E0%B8%B4%E0%B9%80%E0%B8%84%E0%B8%8A%E0%B8%B1%E0%B9%88%E0%B8%99%E0%B8%94%E0%B9%89%E0%B8%A7%E0%B8%A2-JavaScript.aspx?no=9786160825394)

## Introduction
ณ ชั่วโมงนี้ ภาษา **Javascript** อาจจะไม่ใช่ภาษาที่ ~~เร็วที่สุด~~ แต่การเรียนรู้ภาษา JavaScript แค่ภาษาเดียวสามารถที่สร้างสรรค์ผลงานได้อย่างมากมาย เช่น Web Site, Server Site, Destop App, Mobile App, Embedded, Machine Learning, IOT, Game2d/3d และ งานอื่นๆอีกมากมาย เป็นภาษาที่คุ้มที่จะลงทุนศึกษามากที่สุดภาษาหนึ่ง

## Editor for JavaScript
สำหรับ Editor ที่แนะนำให้ใช้ คือ [Visual Studio Code](https://code.visualstudio.com/)
* ติดตั้ง Extensions เพิ่มเติม
  * JavaScript (ES6) code snippets
  * JavaScript Standard Style
  * Live Server
* หากต้องการใช้ Javascript Standard ในการกำหนด format style ให้ติดตั้ง `sudo npm i -g standard`
```json
  // ตั้งค่า vs code ให้จัด format style อัตโนมัติตอนกด save
  {
    "editor.wordWrap": "on",
    "editor.formatOnSave": true,
    "standard.autoFixOnSave": true
  }
```

## Using JavaScript
การเรียกใช้งาน JavaScript

```html
1. External
<body>
  <script src="./app.js"></script>
</body>
```

```html
2. Internal
<body>
  <script>console.log("Hlloe there!")</script>
</body>
```

```html
3. Inline HTML
<body>
   <a href="#" onclick="alert('Hi');">Click Me</a>
</body>
```

## Console Log
```javascript
console.log('Hello')
console.log(1)
console.log(true)
let greeting = 'Hello'
console.log(greeting)
console.log([1, 2, 3, 4])
console.log({a: 1, b: 2, c: '3'})
console.error('This is some error')
console.clear()
console.warn('this is a warning')
console.time('Hello')
  console.log('a')
  console.log('b')
  console.log('c')
console.timeEnd('Hello')

```

## Variables
```javascript
var un
console.log(typeof un) // undefined

var num = 1
console.log(typeof num) // number

var str = 'Yo'
console.log(typeof str) // string

var bool = true
console.log(typeof bool) // boolean

var arr = [1, 2, 3]
console.log(typeof arr) // object

var obj = {}
console.log(typeof obj) // object

var f = function () {}
console.log(typeof f) // function

// การประกาศตัวแปรสามารถขึ้นต้นด้วย _, $ ได้
// ตัวอย่างการประกาศตัวแปรที่ถูกต้อง
var apples
var $apples
var _apples
var app_les
var apples4eva
var apple$

// ตัวอย่างการประกาศตัวแปรที่ไม่ถูกต้อง
var 1apples
var app les
var #apples
var apple%

// variable style
var firstName = 'Yo' // Camel case
console.log(firstName)

```

## Const Let
```javascript
// ES5
var name = 'Jane'
var title = 'Software Engineer'
var hourlyWage = 40

// ES6
const name = 'Jane'

let title = 'Software Engineer'
title = 'Senior Software Engineer'
```

## Data Types in JavaScript
```
String          Arrays
Number          Object Literals
Boolean         Functions
Null            Dates
Undefined       Anything Else...
Symbols(ES6)
```
```javascript
  let un
  console.log(typeof un) // undefined

  let num = 1
  console.log(typeof num) // number

  let str = 'Yo'
  console.log(typeof str) // string

  let bool = true
  console.log(typeof bool) // boolean

  const arr = [1, 2, 3]
  console.log(typeof arr) // object

  const obj = {}
  console.log(typeof obj) // object

  const f = function () {}
  console.log(typeof f) // function

  const sym = Symbol()
  console.log(typeof sym) // symbol
```
## Type Conversion
```javascript
// Number to String
// case 1
let val = String(1)
console.log(val) // "1"

// case 2
let val = 1
console.log(val.toString()) // "1"

// case 3
let val1 = 1
let val2 = String('1')
console.log(val1 + val2) // "11"

// String to Number
// case 1
let val = Number('1')
console.log(val) // 1

// case 2
let val = parseInt('1')
console.log(val) // 1

// case 3
let val = parseFloat('100.33333')
console.log(val.toFixed(2)) // "100.33"
```
## Operators
JavaScript Arithmetic Operators
<table>
<tbody><tr>
<th style="width:12%">Operator</th>
<th style="width:25%">Description</th>
<th>Example</th>
<th>Result in y</th>
<th>Result in x</th>
</tr>
<tr>
<td>+</td>
<td>Addition</td>
<td>x = y + 2</td>
<td>y = 5</td>
<td>x = 7</td>
</tr>
<tr>
<td>-</td>
<td>Subtraction</td>
<td>x = y - 2</td>
<td>y = 5</td>
<td>x = 3</td>
</tr>
<tr>
<td>*</td>
<td>Multiplication</td>
<td>x = y * 2</td>
<td>y = 5</td>
<td>x = 10</td>
</tr>
<tr>
<td>/</td>
<td>Division</td>
<td>x = y / 2</td>
<td>y = 5</td>
<td>x = 2.5</td>
</tr>
<tr>
<td>%</td>
<td>Modulus (division remainder)</td>
<td>x = y % 2</td>
<td>y = 5</td>
<td>x = 1</td>
</tr>
<tr>
<td rowspan="2">++</td>
<td rowspan="2">Increment</td>
<td>x = ++y</td>
<td>y = 6</td>
<td>x = 6</td>
</tr>
<tr style="background-color:#ffffff;">
<td>x = y++</td>
<td>y = 6</td>
<td>x = 5</td>
</tr>
<tr style="background-color:#f1f1f1;">
<td rowspan="2">--</td>
<td rowspan="2">Decrement</td>
<td>x = --y</td>
<td>y = 4</td>
<td>x = 4</td>
</tr>
<tr>
<td>x = y--</td>
<td>y = 4</td>
<td>x = 5</td>
</tr>
</tbody></table>

JavaScript Assignment Operators
> Given that x = 10 and y = 5, the table below explains the assignment operators:
<table>
<tbody><tr>
<th style="width:12%">Operator</th>
<th style="width:25%">Example</th>
<th>Same As</th>
<th>Result in x</th>
</tr>
<tr>
<td>=</td>
<td>x = y</td>
<td>x = y</td>
<td>x = 5</td>
</tr>
<tr>
<td>+=</td>
<td>x += y</td>
<td>x = x + y</td>
<td>x = 15</td>
</tr>
<tr>
<td>-=</td>
<td>x -= y</td>
<td>x = x - y</td>
<td>x = 5</td>
</tr>
<tr>
<td>*=</td>
<td>x *= y</td>
<td>x = x * y</td>
<td>x = 50</td>
</tr>
<tr>
<td>/=</td>
<td>x /= y</td>
<td>x = x / y</td>
<td>x = 2</td>
</tr>
<tr>
<td>%=</td>
<td>x %= y</td>
<td>x = x % y</td>
<td>x = 0</td>
</tr>
</tbody></table>

Comparison Operators
> Comparison operators are used in logical statements to determine equality or difference between variables or values. Given that x = 5, the table below explains the comparison operators:
<table>
<tbody><tr>
<th style="width:12%">Operator</th>
<th>Description</th>
<th>Comparing</th>
<th>Returns</th>
</tr>
<tr style="background-color:#f5f5f5;">
<td rowspan="2">==</td>
<td rowspan="2">equal to</td>
<td>x == 8</td>
<td>false</td>
</tr>
<tr style="background-color:#f5f5f5;">
<td>x == 5</td>
<td>true</td>
</tr>
<tr style="background-color:#ffffff;">
<td rowspan="2">===</td>
<td rowspan="2">equal value and equal type</td>
<td>x === "5"</td>
<td>false</td>
</tr>
<tr style="background-color:#ffffff;">
<td>x === 5</td>
<td>true</td>
</tr>
<tr>
<td>!=</td>
<td>not equal</td>
<td>x != 8</td>
<td>true</td>
</tr>
<tr>
<td rowspan="2">!==</td>
<td rowspan="2">not equal value or not equal type</td>
<td>x !== "5"</td>
<td>true</td>
</tr>
<tr style="background-color:#ffffff;">
<td>x !== 5</td>
<td>false</td>
</tr>
<tr style="background-color:#f5f5f5;">
<td>&gt;</td>
<td>greater than</td>
<td>x &gt; 8</td>
<td>false</td>
</tr>
<tr style="background-color:#ffffff;">
<td>&lt;</td>
<td>less than</td>
<td>x &lt; 8</td>
<td>true</td>
</tr>
<tr style="background-color:#f5f5f5;">
<td>&gt;=</td>
<td>greater than or equal to</td>
<td>x &gt;= 8</td>
<td>false</td>
</tr>
<tr style="background-color:#ffffff;">
<td>&lt;=</td>
<td>less than or equal to</td>
<td>x &lt;= 8</td>
<td><em>true</em></td>
</tr>
</tbody></table>

Logical Operators
> Given that x = 6 and y = 3, the table below explains the logical operators:
<table>
<tbody><tr>
<th style="width:12%">Operator</th>
<th>Description</th>
<th>Example</th>
</tr>
<tr>
<td>&amp;&amp;</td>
<td>and</td>
<td> (x &lt; 10 &amp;&amp; y &gt; 1) is true</td>
</tr>
<tr>
<td>||</td>
<td>or</td>
<td>(x === 5 || y === 5) is false</td>
</tr>
<tr>
<td>!</td>
<td>not</td>
<td> !(x === y) is true</td>
</tr>
</tbody></table>

JavaScript Bitwise Operators
<table>
<tbody><tr>
<th style="width:12%">Operator</th>
<th style="width:25%">Description</th>
<th>Example</th>
<th>Same as</th>
<th>Result</th>
<th style="width:15%">Decimal</th>
</tr>
<tr>
<td>&amp;</td>
<td>AND</td>
<td>x = 5 &amp; 1</td>
<td>0101 &amp; 0001</td>
<td>0001</td>
<td>&nbsp;1</td>
</tr>
<tr>
<td>|</td>
<td>OR</td>
<td>x = 5 | 1</td>
<td>0101 | 0001</td>
<td>0101</td>
<td>&nbsp;5</td>
</tr>
<tr>
<td>~</td>
<td>NOT</td>
<td>x = ~ 5</td>
<td>&nbsp;~0101</td>
<td>1010</td>
<td>&nbsp;10</td>
</tr>
<tr>
<td>^</td>
<td>XOR</td>
<td>x = 5 ^ 1</td>
<td>0101 ^ 0001</td>
<td>0100</td>
<td>&nbsp;4</td>
</tr>
<tr>
<td>&lt;&lt;</td>
<td>Left shift</td>
<td>x = 5 &lt;&lt; 1</td>
<td>0101 &lt;&lt; 1</td>
<td>1010</td>
<td>&nbsp;10</td>
</tr>
<tr>
<td>&gt;&gt;</td>
<td>Right shift</td>
<td>x = 5 &gt;&gt; 1</td>
<td>0101 &gt;&gt; 1</td>
<td>0010</td>
<td>&nbsp; 2</td>
</tr>
</tbody></table>

## Math
```javascript
console.log(Math.PI) // 3.141592653589793
console.log(Math.E) // 2.718281828459045
console.log(Math.round(2.4)) // 2
console.log(Math.ceil(2.4)) // 3
console.log(Math.floor(2.4)) // 2
console.log(Math.sqrt(64)) // 8
console.log(Math.abs(-3)) // 3
console.log(Math.pow(8, 2)) // 64
console.log(Math.min(1, 2, 3)) // 1
console.log(Math.max(1, 2, 3)) // 3
console.log(Math.random())
console.log(Math.floor(Math.random() * 20 + 1))
```

## String Method
```javascript
let name = 'YoProgrammer'
console.log(name.length) // 12

let name = 'YoProgrammer'
console.log(name.toUpperCase()) // "YOPROGRAMMER"

let name = 'YoProgrammer'
console.log(name.toLowerCase()) // "yoprogrammer"

let name = "YoProgrammer"
console.log(name.charAt(2)) // "P"

let name = "YoProgrammer"
console.log(name.substring(0, 4)) // "YoPr"

let name = "YoProgrammer"
console.log(name.replace("Programmer", "Developer")) // "YoDeveloper"

let name = "YoProgrammer"
console.log(name.includes("Yo")) // true
console.log(name.includes("Yea")) // false
```

## index of
```javascript
const arr = ['apple', 'banana', 'orange']
console.log(arr.indexOf('banana')) // 1 นับจากซ้ายไปขวา -> 0, 1
console.log(arr.indexOf('no')) // -1
```

## last index of
```javascript
const arr = ['apple', 'banana', 'orange']
console.log(arr.lastIndexOf('banana')) // 1 นับจากขวาไปซ้าย  1, 0 <-
console.log(arr.lastIndexOf('no')) // -1
```

## Concat
```javascript
let arr1 = [1, 2, 3];
let arr2 = [4, 5, 6];
let sum = arr1.concat(arr2);
console.log(sum);
//output
//[ 1, 2, 3, 4, 5, 6 ]
```

## Template Strings
```javascript
function getMessage() {
  const year = new Date().getFullYear()
  return `The year is ${year}`
}

console.log(getMessage())
```

## Array Helper Methods
## Join
```javascript
let arr = [1, 2, 3, 4, 5];
console.log(arr.join(''));
console.log(arr.join(','));
console.log(arr.join('-'));
//output
// 12345
// 1,2,3,4,5
// 1-2-3-4-5
```

## Push
```javascript
let color = ['red', 'green'];
let mutate = color.push('blue');
console.log(color);
console.log(mutate);
//output
// [ 'red', 'green', 'blue' ]
// 3
```

## Pop
```javascript
let color = ['red', 'green', 'blue'];
let mutate = color.pop('blue');
console.log(color);
console.log(mutate);
//output
// [ 'red', 'green' ]
// blue
```

## Shift
```javascript
let color = ['red', 'green', 'blue'];
let mutate = color.shift();
console.log(color);
console.log(mutate);
//output
// [ 'green', 'blue' ]
// red
```

## Unshift
```javascript
let color = ['red', 'green', 'blue'];
let mutate = color.unshift('ogrange');
console.log(color);
console.log(mutate);
//output
// [ 'ogrange', 'red', 'green', 'blue' ]
// 4
```

## Splice
```javascript
let color = ['ogrange', 'red', 'green', 'blue'];

//ตัวอย่างที่ 1
// let mutate = color.splice(1); //ลบตั้งแต่ตำแหน่งที่ 1 เป็นต้นไป

//ตัวอย่างที่ 2
// let mutate = color.splice(1, 1); //ลบตั้งแต่ตำแหน่งที่ 1 ไป 1 ตัว

//ตัวอย่างที่ 3
let mutate = color.splice(1, 1, 'white', 'black'); // ลบตั้งแต่ตำแหน่งที่ 1 ไป 1 ตัว และเพิ่ม element เข้าไปตำแหน่งที่ 1

console.log(color);
console.log(mutate);

//output
//ตัวอย่างที่ 1
// [ 'ogrange' ]
// [ 'red', 'green', 'blue' ]

//ตัวอย่างที่ 2
// [ 'ogrange', 'green', 'blue' ]
// [ 'red' ]

//ตัวอย่างที่ 3
// [ 'ogrange', 'white', 'black', 'green', 'blue' ]
// [ 'red' ]
```

## Slice
```javascript
let color = ['red', 'green', 'blue'];

//ตัวอย่างที่ 1
// let slice = color.slice(1);

//ตัวอย่างที่ 2
let slice = color.slice(1, 2); //เลือก element ตั้งแต่ตำแหน่งที่ 1 จนถึง 2 แต่ไม่รวม 2

console.log(color);
console.log(slice);

//output
//ตัวอย่างที่ 1
// [ 'red', 'green', 'blue' ]
// [ 'green', 'blue' ]

//ตัวอย่างที่ 2
// [ 'red', 'green', 'blue' ]
// [ 'green' ]
```

## Split
```javascript
let number = 12345;
console.log(number.toString().split(""))

//output
// [ '1', '2', '3', '4', '5' ]
```

## forEach
```javascript
var colors = ['red', 'green', 'blue']

// for
console.log('=== for ===')
for (var i = 0; i < colors.length; i++) {
  console.log(colors[i])
}

// forEach
console.log('=== forEach ===')
colors.forEach(color => console.log(color))

// forEach Continued
console.log('=== forEach Continued ===')
var numbers = [1,2,3,4,5]
var sum = 0
numbers.forEach(number => sum += number)
console.log(sum)

// Exercise
console.log('=== Execrcise ===')
var images = [
  { height: 10, width: 30 },
  { height: 20, width: 90 },
  { height: 54, width: 32 }
];
var areas = [];

images.forEach(function(image) {
  areas.push(image.height * image.width)
})

console.log(areas)
```

## map
```javascript
var numbers = [1, 2, 3]
var doubleNumbers = []

// for
console.log('=== for ===')
for (var i = 0; i < numbers.length; i++) {
  doubleNumbers.push(numbers[i] * 2)
}
console.log(doubleNumbers)

// map
console.log('=== map ===')
var doubled = numbers.map(number => number * 2)
console.log(doubled)

// map Continued
var cars = [
  { model: 'Buick', price: 'CHEAP'},
  { model: 'Camaro', price: 'expensive'}
]
var prices = cars.map(car => car.price)
console.log(prices)

// Exercise 1
console.log('=== Execrcise 1 ===')
var images = [
  { height: '34px', width: '39px' },
  { height: '54px', width: '19px' },
  { height: '83px', width: '75px' },
];

var heights = images.map(image => image.height)
console.log(heights)

// Exercise 2
console.log('=== Execrcise 2 ===')
var trips = [
  { distance: 34, time: 10 },
  { distance: 90, time: 50 },
  { distance: 59, time: 25 }
];

var speeds = trips.map(trip => trip.distance / trip.time)
console.log(speeds)

// Exercise 3
console.log('=== Execrcise 3 ===')
var paints = [ { color: 'red' }, { color: 'blue' }, { color: 'yellow' }];
pluck(paints, 'color'); // returns ['red', 'yellow', 'blue'];
function pluck(array, property) {
  let paints = array.map(prop => prop[property])
  console.log(paints)
  return paints
}
```

## filter
```javascript
var products = [
  { name: 'cucumber', type: 'vegetable', quantity: 0, price: 1 },
  { name: 'banana', type: 'fruit', quantity: 0, price: 1 },
  { name: 'celely', type: 'vegetable', quantity: 0, price: 1 },
  { name: 'orange', type: 'fruit', quantity: 0, price: 1 },
]

var filterdProducts = []

// for
console.log('=== for ===')
for (var i = 0; i < products.length; i++) {
  if (products[i].type === 'fruit') {
    filterdProducts.push(products[i])
  }
}
console.log(filterdProducts)

// filter
console.log('=== filter ===')
var newProducts = products.filter(product => product.type === 'fruit')
console.log(newProducts)

// Choosting When to Filter
var post = {id:4, title: 'New Post'}
var comments = [
  {postId: 4, content: 'awesome post'},
  {postId: 3, content: 'it was ok'},
  {postId: 4, content: 'neat'},
]
// filter Continued
console.log('=== filter Continued ===')
function commentsForPost(post, comments) {
  return comments.filter(comment => comment.postId === post.id)
}
var res = commentsForPost(post, comments)
console.log(res)

// Exercise 1 filter number over 50
console.log('=== Execrcise 1 ===')
var numbers = [15, 25, 35, 45, 55, 65, 75, 85, 95];
var filteredNumbers = numbers.filter(number => number > 50)
console.log(filteredNumbers)

// Exercise 2 filter user admin = true
console.log('=== Execrcise 2 ===')
var users = [
  { id: 1, admin: true },
  { id: 2, admin: false },
  { id: 3, admin: false },
  { id: 4, admin: false },
  { id: 5, admin: true },
]
var filteredUsers = users.filter(user => user.admin)
console.log(filteredUsers)

// Exercise 3 reject number over 15
console.log('=== Execrcise 3 ===')
var numbers = [10, 20, 30, 12]
var lessThanFifteen = reject(numbers, function(number){
  return number > 15
})
function reject(array, iteratorFunction) {
  // คิดแบบ for
  // let newArray = []
  // for (var i = 0; i < array.length; i++) {
  //   if ( ! iteratorFunction(numbers[i])) {
  //     newArray.push(numbers[i])
  //   }
  // }
  // return newArray

  return array.filter(number => ! iteratorFunction(number))
}
console.log(lessThanFifteen)
```

## find
```javascript
var users = [
  {name: 'Jill'},
  {name: 'Alex', id: 4},
  {name: 'Bill'},
  {name: 'Alex'},
]

var user
console.log('=== for ===')
for (var i = 0; i < users.length; i++) {
  if (users[i].name === 'Alex') {
    user = users[i]
    break
  }
}
console.log(user)

console.log('=== find ===')
var findUser = users.find(user => user.name === 'Alex')
console.log(findUser)

console.log('=== find Continued 1 ===')
function Car(model) {
  this.model = model
}
var cars = [
  new Car('Buick'),
  new Car('Camaro'),
  new Car('Focus'),
]

var findCar = cars.find(car => car.model === 'Focus')
console.log(findCar)

console.log('=== find Continued 2 ===')
var posts = [
  {id: 1, title: 'New Post'},
  {id: 2, title: 'Old Post'}
]
var comment = {postId: 1, content: 'Great Post'}
function postForComment(posts, comment) {
  return posts.find(post => post.id === comment.postId)
}

var findPost = postForComment(posts, comment)
console.log(findPost)

// Exercise 1 find admin
console.log('=== Execrcise 1 ===')
var users = [
  { id: 1, admin: false },
  { id: 2, admin: false },
  { id: 3, admin: true }
];

var admin = users.find(user => user.admin)
console.log(admin)

// Exercise 2 balance of 12
console.log('=== Execrcise 2 ===')
var accounts = [
  { balance: -10 },
  { balance: 12 },
  { balance: 0 }
];

var account = accounts.find(account => account.balance === 12)
console.log(account)

// Exercise 3 find by property
console.log('=== Execrcise 3 ===')
var ladders = [
  { id: 1, height: 20 },
  { id: 3, height: 25 }
]

function findWhere(array, criteria) {
  var property = Object.keys(criteria)[0]
  return array.find(ladder => {
    return ladder[property] === criteria[property]
  })
}

var res = findWhere(ladders, { height: 25 })
console.log(res)
```

## find index
```javascript
const arr = ['apple', 'banana', 'orange']
console.log(arr.findIndex(e => e === 'banana')) // output = 1
```

## every and some
```javascript
var computers = [
  {name: 'Apple', ram: 24},
  {name: 'Compaq', ram: 4},
  {name: 'Acer', ram: 32}
]

var allComputersCanRunProgram = true
var onlySomeComputersCanRunProgram = false

console.log('=== for ===')
for (var i = 0; i < computers.length; i++) {
  var computer = computers[i]
  if (computer.ram < 16) {
    allComputersCanRunProgram = false
  } else {
    onlySomeComputersCanRunProgram = true
  }
}

console.log(allComputersCanRunProgram)
console.log(onlySomeComputersCanRunProgram)

console.log('=== every ===')
var everyComputers = computers.every(computer => computer.ram > 16)
console.log(everyComputers)

console.log('=== some ===')
var someComputers = computers.some(computer => computer.ram > 16)
console.log(someComputers)

// Every and Some in Practice
console.log('=== Practice ===')
function Field(value) {
  this.value = value
}
Field.prototype.validate = function() {
  return this.value.length > 0
}
var username = new Field("2cool")
var password = new Field("my_password")
var birthdate = new Field("10/10/2010")

var fields = [username, password, birthdate]
var formIsValid = fields.every(field => field.validate())

if (formIsValid) {
  // allow user to submit!
  console.log('formIsValid', formIsValid)
} else {
  // show an error message!
  console.log('formIsValid', formIsValid)
}

// Exercise 1 validate hasSubmitted
console.log('=== Execrcise 1 ===')
var users = [
  { id: 21, hasSubmitted: true },
  { id: 62, hasSubmitted: false },
  { id: 4, hasSubmitted: true }
];

var hasSubmitted = users.every(user => user.hasSubmitted)
console.log(hasSubmitted)

// Exercise 2 assign the boolean 'true' to the variable 'inProgress'
console.log('=== Execrcise 2 ===')
var requests = [
  { url: '/photos', status: 'complete' },
  { url: '/albums', status: 'pending' },
  { url: '/users', status: 'failed' }
];

var inProgress = requests.some(request => request.status === 'complete')
console.log(inProgress)
```

## reduce
```javascript
var numbers = [10, 20, 30]
var sum = 0

console.log('=== for ===')
for (var i = 0; i < numbers.length; i++) {
  sum += numbers[i]
}
console.log(sum)

console.log('=== reduce ===')
var r = numbers.reduce((previous, number) => previous + number, 0)
console.log(r)

// A touch More of Reduce
var primaryColors = [
  {color: 'red'},
  {color: 'green'},
  {color: 'blue'},
]

console.log('=== reduce Continued ===')
var p = primaryColors.reduce(function(previos, primaryColor){
  previos.push(primaryColor.color)
  return previos
}, [])

console.log(p)

console.log('=== reduce Continued 2 ===')
function balancedParens(string) {
  return string.split("").reduce((previous, char) => {
    if (previous <= 0) { return previous }
    if (char === "(") { return ++previous }
    if (char === ")") { return --previous }
    return previous
  }, 0)
}
var b= balancedParens(")))))")
console.log(b)

// Exercise 1 reduce sum distance
console.log('=== Excercise 1 ===')
var trips = [{ distance: 34 }, { distance: 12 } , { distance: 1 }];
var totalDistance = trips.reduce((previos, trip) => previos + trip.distance, 0)
console.log(totalDistance)

// Exercise 2 ต้องการผลลัพธ์ = { sitting: 3, standing: 2 }
console.log('=== Excercise 2 ===')
var desks = [
  { type: 'sitting' },
  { type: 'standing' },
  { type: 'sitting' },
  { type: 'sitting' },
  { type: 'standing' }
];

var deskTypes = desks.reduce(function(previos, desk) {
    if (desk.type === 'sitting') { ++previos.sitting }
    if (desk.type === 'standing') { ++previos.standing }
    return previos
}, { sitting: 0, standing: 0 });
console.log(deskTypes)

// Exercise 3 unique value by reduc & find
console.log('=== Excercise 3 ===')
var numbers = [1, 1, 2, 3, 4, 4]

function unique(array) {
  return array.reduce(function(previos, arr){
    if (previos.find(p => p === arr)) {
      return previos
    }
    previos.push(arr)
    return previos
  }, [])
}
console.log(unique(numbers))
```

## sort
```javascript
// Sort String
let fruit = ['cherries', 'apples', 'bannas'];
console.log(fruit.sort()); // [ 'apples', 'bannas', 'cherries' ]

// Sort Number
let scores = [1, 10, 21, 2];
console.log(scores.sort()); //[1, 10, 21, 2];

let numbers = [4, 2, 10, 5, 1, 3];
numbers.sort(function(a, b) {
  return a - b;
});
console.log(numbers); //[ 1, 2, 3, 4, 5, 10]

// Sort Object
let items = [
  { name: 'Edward', value: 21 },
  { name: 'Sharpe', value: 37 },
  { name: 'And', value: 45 },
  { name: 'The', value: -12 },
  { name: 'Magnetic', value: 13 },
  { name: 'Zeros', value: 37 }
];

// sort object by value
items.sort(function (a, b) {
  return a.value - b.value;
});
console.log(items);
//output
// [ { name: 'The', value: -12 },
// { name: 'Magnetic', value: 13 },
// { name: 'Edward', value: 21 },
// { name: 'Sharpe', value: 37 },
// { name: 'Zeros', value: 37 },
// { name: 'And', value: 45 } ]


// sort object by name
items.sort(function(a, b) {
  let nameA = a.name.toUpperCase(); // ignore upper and lowercase
  let nameB = b.name.toUpperCase(); // ignore upper and lowercase
  if (nameA < nameB) {
    return -1;
  }
  if (nameA > nameB) {
    return 1;
  }

  // names must be equal
  return 0;
});
console.log(items);
//output
// [ { name: 'And', value: 45 },
// { name: 'Edward', value: 21 },
// { name: 'Magnetic', value: 13 },
// { name: 'Sharpe', value: 37 },
// { name: 'The', value: -12 },
// { name: 'Zeros', value: 37 } ]
```

## Arrow Function
```javascript
const add = (a, b) => a + b
console.log(add(1, 2))

const numbers = [1, 2, 3]
console.log(numbers.map(n => n * 2))

// function () { local scope } ต้อง => bind(this)
// const team = {
//   members: ['Jane', 'Bill'],
//   teamName: 'Super Squad',
//   teamSummary: function() {
//     return this.members.map(function(member) {
//       return `${member} is on team ${this.teamName}`
//     }.bind(this))
//   }
// }

const team = {
  members: ['Jane', 'Bill'],
  teamName: 'Super Squad',
  teamSummary: function() {
    return this.members.map((member) => {
      return `${member} is on team ${this.teamName}`
    })
  }
}

console.log(team.teamSummary())

const profile = {
  name: 'Alex',
  getName: function() {return this.name;}
}

console.log(profile.getName())

```

## Enhanced Object Literals
```javascript
function createBookShop(inventory) {
  return {
    inventory, // inventory: inventory
    inventoryValue() { // inventoryValue: function()
      return this.inventory.reduce((total, book) => total + book.price, 0)
    },
    priceForTitle(title){ // priceForTitle: function(title)
      return this.inventory.find(book => book.title === title).price
    }
  }
}

const inventory = [
  {title: 'Harry Potter', price: 10},
  {title: 'Eloquent Javascript', price: 15}
]

const bookShop = createBookShop(inventory)
console.log(bookShop.inventoryValue())
console.log(bookShop.priceForTitle('Harry Potter'))
```

## Default Function Argument
```javascript
function makeAjaxRequest(url, method = 'GET') {
  return method
}
console.log(makeAjaxRequest('google.com')) // null != undefined
console.log(makeAjaxRequest('google.com', 'POST'))

function User(id) {
  this.id = id
}

function generateId() {
  return Math.random() * 9999999
}

function createAdminUser(user = new User(generateId())) {
  user.admin = true
  return user
}

console.log(createAdminUser())
```

## Capturing Arguments
```javascript
console.log('=== capturing ===')
function addNumbers(...numbers) {
  return numbers.reduce((sum, number) => sum + number, 0)
}
console.log(addNumbers(1,2,3,4,5))

const defaultColors = ['red', 'green']
const userFavoriteColors = ['orange', 'yellow']

console.log('=== concat ===')
console.log(defaultColors.concat(userFavoriteColors))

console.log('=== rest ===')
console.log([...defaultColors, ...userFavoriteColors])

console.log('=== spread ===')
function validateShoppingList(...items) {
  if (items.indexOf('milk') < 0) {
    return [ 'milk', ...items]
  }
  return items
}
console.log(validateShoppingList('oranges', 'bread', 'eggs'))

console.log('=== Exercise 1 ===')
var array = [1, 2]
var array2 = [3, 4, 5]

console.log('=== normal ===')
function unshift(array, a, b, c, d, e) {
  return [a, b, c, d, e].concat(array);
}

console.log(unshift(array, 3,4,5,6,7))

// Refactor
console.log('=== rest ===')
function unshiftRefactor(array, ...array2) {
  return [...array, ...array2];
}
console.log(unshiftRefactor(array, 3,4,5,6,7))
```

## Destructuring
```javascript
var expense = {
  type: 'Business',
  amount: '$45 USD'
}

// ES5
// var type = expense.type
// var amount = expense.amount

// ES6
const { type, amount } = expense
console.log(type, amount) // output: Business $45 USD

var savedFiled = {
  extension: 'jpg',
  name: 'repost',
  size: 14040
}

function fileSummary({name, extension, size}, {color}) {
  return `The file ${name}.${extension} is of size ${size} color ${color}`
}
console.log(fileSummary(savedFiled, {color: 'red'}))
// output: The file repost.jpg is of size 14040 color red

const companies = [
  'Google',
  'Facebook',
  'Uber'
]

console.log('=== destructuring array ===')
const [name, name2, name3] = companies
console.log(name, name2, name3)
const [...rest] = companies
console.log(rest)

console.log('=== destructuring object ===')
const companies2 = [
  {name: 'Google', location: 'Mountain View'},
  {name: 'Facebook', location: 'Menlo Park'},
  {name: 'Uber', location: 'San Francisco'},
]
const [{location}] = companies2
console.log(location)

const Google = {
  locations: ['Mountain View', 'New York']
}

const {locations: [fLocation]} = Google
console.log(fLocation)

console.log('=== destructuring Continued ===')
function signup({username, password, email, dateOfBirth, city}) {
  return username
}
const user = {
  username: 'myname',
  password: 'mypassword',
  email: 'myemail@example.com',
  dateOfBirth: '1/1/1900',
  city: 'New York'
}
console.log(signup(user))

console.log('=== destructuring Continued 2 ===')
const points = [
  [4, 5],
  [10, 1],
  [0, 40],
]

console.log(points.map(([x, y]) => ({x, y})))
// output [ { x: 4, y: 5 }, { x: 10, y: 1 }, { x: 0, y: 40 } ]

console.log('=== Exercies 1 ===')
// ต้องการผลลัพธ์
// [ { subject: 'Chemistry', time: '9AM', teacher: 'Mr. Darnick' },
//   { subject: 'Physics', time: '10:15AM', teacher: 'Mrs. Lithun' },
//   { subject: 'Math', time: '11:30AM', teacher: 'Mrs. Vitalis' } ]
const classes = [
  [ 'Chemistry', '9AM', 'Mr. Darnick' ],
  [ 'Physics', '10:15AM', 'Mrs. Lithun'],
  [ 'Math', '11:30AM', 'Mrs. Vitalis' ]
];

const classesAsObject = classes.map(([subject, time, teacher]) => ({
  subject, time, teacher
}))
console.log(classesAsObject)

console.log('=== Exercies 2 ===')
// ต้องการ output [2,4,6] โดยห้ามใช้ helper array เช่น map, forEach, reduce
const numbers = [1, 2, 3];

function double([...array]) {
  var newArray = []
  for (var i = 0; i < array.length; i++) {
    newArray[i] = array[i] * 2
  }
  return newArray
}
console.log(double(numbers))
```

## Classes
```javascript
console.log('=== classes introduction ===')
function Car(options) {
  this.title = options.title
}

Car.prototype.drive = function() {
  return 'vroom'
}

const car = new Car({title: 'Focus'})

console.log(car.drive())
console.log(car.title)
```

## Prototypal Inheritance
```javascript
console.log('=== prototypal inheritance ===')
function Car(options) {
  this.title = options.title
}

Car.prototype.drive = function() {
  return 'vroom'
}

function Toyota(options) {
  Car.call(this, options)
  this.color = options.color
}

Toyota.prototype = Object.create(Car.prototype)
Toyota.prototype.constructor = Toyota

Toyota.prototype.honk = function() {
  return 'beep'
}

const toyota = new Toyota({color: 'red', title: 'Daily Driver'})
console.log(toyota.drive())
console.log(toyota.color)
console.log(toyota.title)
console.log(toyota.honk())
```

## Refactoring with Classes
```javascript
console.log('=== refactoring classes ===')

class Car {
  constructor(options) {
    this.title = options.title
  }

  drive() {
    return 'vroom'
  }
}

const car = new Car({title: 'Honda'})
console.log(car)
console.log(car.drive())
console.log(car.title)

class Toyota extends Car {
  constructor(options) {
    super(options)
    this.color = options.color
  }
  honk() {
    return 'beep'
  }
}
const toyota = new Toyota({title: 'Toyota', color: 'red'})
console.log(toyota)
console.log(toyota.drive())
console.log(toyota.title)
console.log(toyota.honk())
console.log(toyota.color)

console.log('=== Exercise 1 ===')
class Monster {
  constructor(options) {
    this.name = options.name
    this.health= 100
  }
}

console.log('=== Exercise 2 ===')
class Monster2 {
  constructor(options) {
    this.health = 100;
    this.name = options.name;
  }
}

class Snake extends Monster2{
  constructor(options){
    super(options)
  }
  bite() {
    this.health -= 10
  }
}

const snake = new Snake({name: 'Snake'})
snake.bite()
console.log(snake.health)
```

## Callback
ตัวอย่างการใช้ callback ใน express.js
```javascript
const express = () => {
  return {
    use: (path, cb) => {
      const error = {}
      const req = {
        path: path
      }
      const res = {}
      const next = {}
      cb(error, req, res, next)
    }
  }
}

const app = express()

app.use('/api', (error, req, res, next) => {
  console.log(error, req, res, next)
})

// output
[object Object] { ... }
[object Object] {
  path: "/api"
}
[object Object] { ... }
[object Object] { ... }
```

ตัวอย่างการใช้งาน callback synchronous
```javascript
console.log('Start')
var getUser = (id, cb) => {
  var user = {
    id: id,
    name: 'Yo'
  }
  cb(user)
}

getUser(1, (user) => {
  console.log(user)
})

console.log('End')

======
Output
======
Start
{ id: 1, name: 'Yo' }
End
```

ตัวอย่างการใช้งาน callback Asynchronous
```javascript
console.log('Start')
var getUser = (id, cb) => {
  var user = {
    id: id,
    name: 'Yo'
  }
  setTimeout(() => {
    cb(user)
  }, 2000)
}

getUser(1, (user) => {
  console.log(user)
})

console.log('End')

======
Output
======
Start
End
---------------------- delay 2000ms
{ id: 1, name: 'Yo' }
```


ตัวอย่างการใช้งาน callback Asynchronous และต้องการเรียงลำดับความถูกต้อง
```javascript
function Open(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`1. เปิดประตู ${rand}ms`)
  }, rand)
}

function Order(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`2. สั่งกาแฟ ${rand}ms`)
  }, rand)
}

function Sit(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`3. หาที่นั่ง ${rand}ms`)
  }, rand)
}

function Drink(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`4. ดื่มกาแฟ ${rand}ms`)
  }, rand)
}

function Pay(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`5. จ่ายเงิน ${rand}ms`)
  }, rand)
}

function Exit(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`6. ออกจากร้าน ${rand}ms`)
  }, rand)
}

function Rand() {
  return (Math.floor(Math.random() * 5) + 1) * 1000
}

// ไม่เรียงตามลำดับ, blocking io
// Open(res => console.log(res))
// Order(res => console.log(res))
// Sit(res => console.log(res))
// Drink(res => console.log(res))
// Pay(res => console.log(res))
// Exit(res => console.log(res))

//เรียงลำดับถูกต้อง, blocking io เกิดสิ่งที่เรียกว่า callback hell
Open(res => {
  console.log(res)
  Order(res => {
    console.log(res)
    Sit(res => {
      console.log(res)
      Drink(res => {
        console.log(res)
        Pay(res => {
          console.log(res)
          Exit(res => {
            console.log(res)
          })
        })
      })
    })
  })
})
```

## Recursive Function
```javascript
function Open(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`1. Open the Door ${rand}ms`)
  }, rand)
}

function Order(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`2. Order a Coffee ${rand}ms`)
  }, rand)
}

function Sit(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`3. Sitdown ${rand}ms`)
  }, rand)
}

function Drink(cup, cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`${cup} ${rand}ms`)
  }, rand)
}

function Pay(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`5. Pay Money ${rand}ms`)
  }, rand)
}

function Exit(cb) {
  let rand = Rand()
  setTimeout(() => {
    cb(`6. Exit Shop ${rand}ms`)
  }, rand)
}

function Rand() {
  return (Math.floor(Math.random() * 3) + 1) * 1000
}

function RecursiveDrink(arrCoffee, cb) {
  if (arrCoffee.length > 0) {
    let cup = arrCoffee.shift()
    Drink(cup, res => {
      console.log(res)
      RecursiveDrink(arrCoffee, cb)
    })
  } else {
    cb('Drink Success')
  }
}

Open(res => {
  console.log(res)
  Order(res => {
    console.log(res)
    Sit(res => {
      console.log(res)
      console.log('4. Drink Coffee')
      RecursiveDrink(['4.1. Espresso', '4.2. Late', '4.3. Back Coffee'], res => {
        console.log(res)
        Pay(res => {
          console.log(res)
          Exit(res => {
            console.log(res)
          })
        })
      })
    })
  })
})
```

## Promise
```javascript
const Open = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`1. เปิดประตู ${rand}ms`)
  }, rand) 
})

const Order = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`2. สั่งกาแฟ ${rand}ms`)
  }, rand) 
})

const Sit = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`3. หาที่นั่ง ${rand}ms`)
  }, rand) 
})

const Drink = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`4. ดื่มกาแฟ ${rand}ms`)
  }, rand) 
})

const Pay = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`5. จ่ายตังค์ ${rand}ms`)
  }, rand) 
})

const Exit = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`6. ออกจากร้าน ${rand}ms`)
  }, rand) 
})

function Rand() {
  return (Math.floor(Math.random() * 1) + 1) * 1000
}

// ไม่เรียงลำดับ, non blocking io
// Open.then(res => console.log(res))
// Order.then(res => console.log(res))
// Sit.then(res => console.log(res))
// Drink.then(res => console.log(res))
// Pay.then(res => console.log(res))
// Exit.then(res => console.log(res))

// เรียงตามลำดับ, non blocking io
Open
.then(res => {
  console.log(res)
  return
}).then(() => {
  Order
  .then(res => {
    console.log(res)
    return
  })
}).then(() => {
  Sit
  .then(res => {
    console.log(res)
    return
  })
}).then(() => {
  Drink
  .then(res => {
    console.log(res)
    return
  })
}).then(() => {
  Pay
  .then(res => {
    console.log(res)
    return
  })
}).then(() => {
  Exit
  .then(res => {
    console.log(res)
    return
  })
})

======
Output
======
1. เปิดประตู 1000ms
2. สั่งกาแฟ 1000ms
3. หาที่นั่ง 1000ms
4. ดื่มกาแฟ 1000ms
5. จ่ายตังค์ 1000ms
6. ออกจากร้าน 1000m
```

## Async Await
```javascript
const Open = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`1. เปิดประตู ${rand}ms`)
  }, rand) 
})

const Order = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`2. สั่งกาแฟ ${rand}ms`)
  }, rand)
})

const Sit = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`3. หาที่นั่ง ${rand}ms`)
  }, rand) 
})

const Drink = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`4. ดื่มกาแฟ ${rand}ms`)
  }, rand) 
})

const Pay = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`5. จ่ายตังค์ ${rand}ms`)
  }, rand) 
})

const Exit = new Promise((resolve, reject) => {
  let rand = Rand()
  setTimeout(() => {
    resolve(`6. ออกจากร้าน ${rand}ms`)
  }, rand) 
})

function Rand() {
  return (Math.floor(Math.random() * 5) + 1) * 1000
}

// เรียงตามลำดับ, non blocking io
const step = async () => {
  const open = await Open
  console.log(open)

  const order = await Order
  console.log(order)

  const sit = await Sit
  console.log(sit)

  const drink = await Drink
  console.log(drink)

  const pay = await Pay
  console.log(pay)

  const exit = await Exit
  console.log(exit)
}
step()
```

## Reactive
```javascript
function createReactiveObject (obj) {
  const keys = Object.keys(obj)
  obj.$data = Object.assign({}, obj)
  keys.forEach((key) => {
    Object.defineProperty(obj, key, {
      get: reactiveGetter.bind(obj, key),
      set: reactiveSetter.bind(obj, key)
    })
  })
}

function reactiveSetter (property, value) {
  this.$data[property] = value
  console.log(`${property} changed to ${value}`)
}

function reactiveGetter (property) {
  console.log(`get ${property}`)
  return this.$data[property]
}

let user = {
  name: '',
  score: 0
}

createReactiveObject(user)

user.name='Yo'
console.log(user.score) 
```

## Airbnb
A mostly reasonable approach to JavaScript [Click](https://github.com/airbnb/javascript)

## Standard
The best way to learn about standard is to just install it and give it a try on your code. [Click](https://standardjs.com/rules.html)

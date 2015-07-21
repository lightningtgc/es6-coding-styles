# 广发证券ECMAScript6编码规范

> 本规范是基于JavaScript规范上拟定的，只针对ES6相关规范

> 如变量命名，是否加分号等约定的请参考JavaScript的规范

> 应注意目前的代码转换工具(如Babel，traceur)不够完善,有些特性须谨慎使用

## 规范内容

1. [声明 Declarations](#声明)
2. [字符串 Strings](#字符串)
3. [解构 Destructuring](#解构)
4. [数组 Arrays](#数组)
5. [参数依赖... Rest](#参数依赖)
6. [函数 Functions](#函数)
7. [类 Classes](#类)
8. [模块 Modules](#模块)

### 声明
- 1.1 变量

> 对于只在当前作用域下有效的变量，应使用let来代替var

> 对于全局变量声明，采用var，但应避免声明过多全局变量污染环境

```js
// 不好
for (var i=0; i<5; i++) {
  console.log(i);
}
console.log(i);

//好
for (let i=0; i<5; i++) {
  console.log(i);
}
console.log(i);
```

- 1.2 常量

> 对于不再变化的值应使用const，常量命名应遵循字母全大写的通俗约定。

> 应注意const与let只在声明所在的块级作用域内有效。

```js
// 不好
const someNum = 123;
const AnotherStr = '不变的字符串';
let SOME_ARR = ['不','变','数','组'];
var ANOTHER_OBJ = {
  '不变对象': true
};

// 好
const SOME_NUM = 123;
const ANOTHER_STR = '不变的字符串';
const SOME_ARR = ['不','变','数','组'];
const ANOTHER_OBJ = {
  '不变对象': true
};

```

#### 字符串

- 2.1 模板字符串

#### 解构

#### 数组

#### 参数依赖

#### 函数

#### 类

#### 模块




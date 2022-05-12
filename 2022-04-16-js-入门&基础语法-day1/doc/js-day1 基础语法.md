<center><h1>js-day1 基础语法</h1></center>

## 1.js引入方式

- 标签内部式 - 淘汰

  ```html
  1)语法
  	<标签名 事件属性="js代码" > </标签名>
  
  2)案例
  	<div onclick="alert(123)"></div>
  ```

  

- 内嵌式 - 教学

  ```html
  1)语法: 通常在结束body标签之前引入script标签
  2)案例: 
  	<body>
          <script> js代码 </script>
      </body>
  ```

  

- 外链式 - 项目

  ```html
  1)语法: 在结束body标签之前引入外部js文件
  2)案例: 
  	<body>
          <script src="xxx.js"></script>    
  	</body>
  ```

  

## 2. js输出方式

- 网页输出 - 了解

  ```javascript
  document.write()
  ```

- 弹出框输出 - 了解

  ```js
  alert()
  ```

  

- 控制台输出 - 推荐

  ```js
  console.log()
  ```

## 3.变量

- 概念

  ```js
  1) 概念: 保存临时数据的容器
  2) 理解: 在内存中分配很多小空间,并且命名,用于保存程序运行过程中产生的临时数据
  ```

- 三种定义变量以及区别

  ```js
  1) 三种定义方式
  	var   变量 = 值;   淘汰 === 可以重新声明和赋值
  	let   变量 = 值;   推荐 === 不能重新声明,但是可以重新赋值
  	const 变量 = 值;   推荐 === 定义常量,不能重新声明和赋值
  ```

  

- 定义多个变量

  ```js
  let 变量1 = 值,
      变量2 = 值,
      变量n = 值;
  ```

  

- 标识符命名规则

  ```js
  1) 由数字. 字母. 下划线_ 美刀$组成
  2) 不能以数字开头
  3) 不能包含特殊符号
  4) 不能使用关键字和保留字
  5) 驼峰命名法
  6) 字母区分大小写
  ```

  

## 4.数据类型

- 分类

  1. 基本数据类型

     ```js
     number   : 数字
     string   : 字符串
     boolean  : 布尔类型
     undefined: 未定义类型
     null     : 空类型
     symbol   : 符号类型
     ```

     

  2. 引用类型

     ```js
     object
     ```

     

- 类型转换

  1. 强制类型转换

     - 转为number类型

       ```js
       parseInt()    : 转为整数, 不保留小数 
       parseFloat()  : 转为数字, 保留有效位小数
       Number()      : 转为数字
       ```

     - 转为boolean类型

       ```js
       Boolean() : 只有5个值转为false,否则为true   
       		   0 '' undefined null NaN 
       ```

       

     - 转为string类型

       ```js
       String()
       ```

       

  2. 自动类型转换
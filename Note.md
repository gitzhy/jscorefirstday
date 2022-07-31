# JSCORE01

> 小新老师的网站 xin88.top
>
> 包含注意事项 和 联系方式 扫码添加
>
> <img src="JSCORE01.assets/user.jpg" alt="img" style="zoom: 10%;" />

## 阶段内容介绍

> 培训目标: 大前端工程师 - WEB 网页开发 + App 手机端开发 + 小程序开发 + 服务器开发 + PS 切图
>
> - 企业需要 万金油 类型的人才

- 阶段 1 - 成亮
  - 编程基础: 服务器的相关操作 - SQL mysql Express node.js...
- 阶段 2 - 泡泡
  - WEB 开发基础 HTML +CSS + JS + AJAX + 云服务器
    - 能够实现一个 较为好看的 静态页面
    - HTML 负责布局, 层级结构.. CSS 负责美化 (Bootstrap)
- 阶段 3 - 小新老师
  - WEB 开发的核心技术 - JS
  - JS 语言的介入 会让页面带有各种逻辑操作, 与用户之间能够有丰富的交互
  - JS 高级, DOM, jQuery + Vue 框架
- 阶段 4 - 小铭
  - vue 的框架 + 手机端开发 + HTML5 高级 + 大数据 echarts
- 阶段 5 - 文华
  - uniapp 框架 react 框架..
- 阶段 6 - 赠课
  - 高端的 新兴的技术: flutter, webpack, 设计模式....

## 本阶段的一些注意事项

- 学习方式: JS 高级部分 `重在理解`
  - 如果手速慢的同学: 争取先听懂, 理解. 有时间再去写代码
  - 切记!!! 不要为了抄代码 而 放弃听课
- 答疑问题
  - 讲课时间, 讲师不允许 用手机. 有问题尽量找项目经理 -- 不搭理你..你跟老师说.
  - 课下时间, 发消息到 老师的企业微信, 都会一一回复
    - 最好第一句话 先自报家门 : 我是 2205 班的 xx 校区的 xxx
    - 当前班级的同学 消息会优先响应
- 技巧性问题
  - 问问题 一定要 `简单粗暴`, 直接发问题即可, 如果有报错 一定要带 报错截图 + 代码截图
  - 长时间 已读未回, 最好在打个招呼, 发个表情. 可能被忘记了..

## JS 高级

成亮老师讲解的 JS 主要是 简单的使用 偶尔讲解的理论知识`比较浅`

- 第三阶段依然讲解 JS, 但是会深挖底层理论 -- 面试经常问理论知识!

## 作用域和声明

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!-- 题目 就是文件名 -->
    <title>作用域与声明 09:24</title>
  </head>

  <body>
    <!-- 手速慢的话, 不要抄注释. 为了便于同学课下复习, 所以注释会非常多 -->

    <!-- 声明提升: JS的编译器 会先阅读提取代码中的声明操作, 然后提取到作用域的顶部, 然后再执行调整过顺序的代码 -->

    <!-- 目前所有讲解的内容, 都是在 ES6  即JS的第六个版本前的特性 -->
    <!-- 声明操作: var function -->
    <!-- var: 通用的, 可以声明变量, 存储任意类型的值 -->
    <script>
      // var: 声明一个变量, 存储一个值
      var a = 10,
        b = true,
        c = "凯凯",
        d = {},
        e = [];
      var f = function () {};

      // function: 只能声明函数,  声明一个变量来存储函数
      function g() {}

      // 什么是作用域?  就是一个具有特殊作用的对象类型 - JS中 万物皆对象
      // 全局作用域 : 用于存储系统API(函数+变量之类)

      // JS的宿主环境: JS运行在什么环境中,  这个环境就叫宿主
      // 比如 JS运行在 node.js 平台上,  node.js 就是宿主环境
      // JS运行在浏览器上, 浏览器就是 JS 的宿主. JS就能使用浏览器的各种功能

      // 推荐安装 live server 插件,  只要右键 -> open with live server
      // 就能在默认浏览器中开启当前文件
      // 首次使用, 后台有404错误, 不用管. 刷新就没了

      // window中存放了 浏览器提供的所有 API , 可以通过这里的方法来操作浏览器
      console.log("window:", window);

      // alert: 是浏览器提供的最基础的弹窗方法, 其存储在window中
      // window.alert("大家好, 我是alert")

      // 凡是存放在window中的 -- 称为全局对象 或 全局作用域
      // 由于window是专门存储系统API的对象, 所以也称为 作用域
      // window. 可以省略
      alert("大家好, 我是alert");

      // 全局污染: 全局作用域是用来存放系统api的, 如果把我们自己定义的属性放在全局作用域中, 就叫全局污染

      // window是放系统api.
      // 通过var 在 script中声明的变量, 会存储在window中, 称为 全局污染  -- 把自定义的放在系统api存储的地方, 污染了
      var aa = 666;

      // 典型的污染: 除了郑浩 都是讲师,  郑浩污染了这个数组
      // var names = ['成亮', '泡泡', '小新', '铭铭', '郑浩', '文华']

      // 寄生虫 寄生在什么物体上, 这个物体就叫宿主
      // 王力宏感染了 新冠病毒.. 称  王力宏是 新冠病毒的宿主

      // 局部作用域
    </script>
  </body>
</html>
```

## 局部作用域

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>局部作用域 10:14</title>
  </head>

  <body>
    <!-- JS有两个作用域: 全局 和 局部 -->
    <!-- 全局: 在浏览器中就是 window 对象 -->
    <!-- 局部作用域: 函数运行时所产生的对象 -->
    <script>
      // 函数有两种状态: 静态 + 触发态

      // 函数声明后, 处于静止状态: 必须通过调用 -- 函数() 才能触发函数中的代码
      function show() {
        // 变量 a b c 存储在特殊的作用域对象: 函数作用域
        // 函数在运行期间 临时 生成的作用域. 运行结束时会被销毁 来节省内存

        // 浏览器提供了断点调试功能, 可以让代码 中断 在某个时间点, 来查看对应的情况
        var a = 10;
        var b = 20;
        var c = 30;
        // 插件名: JavaScript(ES6) code snippets
        // clg
        console.log(a, b, c);
      }
      // 函数动态: 通过()来触发函数
      show();
      show();
      show();
    </script>
  </body>
</html>
```

## 利用局部作用域解决全局变量污染

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>利用局部作用域解决全局变量污染 10:33</title>
  </head>

  <body>
    <script>
      // 普通写法: 在脚本中声明变量, 会存储在window作用域中, 污染全局
      var a = 10,
        b = 20;
      console.log(a + b); //clg

      // 解决方案: 把代码在函数里执行, 变量自然会存储在函数作用域 而且 函数执行完毕后, 还会释放内存 - 节省内存
      // 全局window 会一直存在到页面关闭, 存储在这里的数据会一直存活

      // 匿名函数自调用 就是专门应对当前场景的技术
      // 为什么匿名: 没有复用的需求, 仅仅是为了执行一次 -- 提供一个局部作用域
      // 注意: 必须和上一行代码之间有分号间隔
      // 理论上: 脚本中书写代码, 开局就该写一个匿名函数, 然后在这里写其他代码
      // 现实中: 很多人不知道 或者 懒, 可能不会这么写, 导致大量的全局污染

      // 字体: monaco

      // 匿名函数的固定格式
      // (function(){})()
      (function () {
        var aa = 10;
        var bb = 20;
        console.log(aa + bb); // 打开全局对象, 看里面有没有aa 和 bb
      })();

      // 查看全局中是否有 a 和 b 两个属性
      console.log("全局:", window);

      // 推荐你 第一天用HBuilder 写,  代码没有任何差别
      // 中午或晚上 看 vscode的视频, 慢慢书写 vscode
    </script>
  </body>
</html>
```

## 插件

<img src="JSCORE01.assets/image-20220729094124782.png" alt="image-20220729094124782" style="zoom:80%;" />

JS 的代码块

![image-20220729101933326](JSCORE01.assets/image-20220729101933326.png)

> 可以一直用 HBuilder 来编写程序, 没有任何影响
>
> VScode 只是另一款编程软件 -- 不强制使用!
>
> ---
>
> 有问题 发企业微信

## 局部作用域

![image-20220729103139750](JSCORE01.assets/image-20220729103139750.png)

![image-20220729105824342](JSCORE01.assets/image-20220729105824342.png)

## 声明提升

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>声明提升 11:18</title>
  </head>

  <body>
    <script>
      // 避免全局变量污染, 开局先书写一个 匿名函数自调用
      // 注意: 匿名函数前通过分号和上一行代码间隔.  没有上一行就不用写分号
      (function () {
        // 代码写在函数中, 所有声明的变量都在函数作用域, 不会污染全局

        // 正常理解:  除了JS以外都是 1111 2222
        // JS独有的 `垃圾` 设定: 导致程序员使用时特别难受
        // JS引擎会隐式把声明代码进行提升, 再执行提升后的代码
        function show() {
          console.log(1111);
        }
        show();

        // 函数: 声明和赋值密不可分, 是一体的
        function show() {
          console.log(2222);
        }
        show();
      })();
    </script>

    <script>
      (function () {
        // var a = 5 //这是两行代码的合写
        // var a;  a = 5;
        // 声明提升: 提升声明的代码
        var a; //声明操作: 声明变量a
        // 赋值操作: a = 函数
        a = function () {
          console.log(1);
        };
        a();

        var a;
        a = function () {
          console.log(2);
        };
        a();
      })();
    </script>

    <script>
      (function () {
        var a = function () {
          console.log(1);
        };
        a();

        var a = function () {
          console.log(2);
        };
        a();

        function a() {
          console.log(3);
        }
        a();
      })();

      // 简化写法
      var a = function () {};

      // 真正的代码
      var a;
      a = function () {};
    </script>
  </body>
</html>
```

![image-20220729113230013](JSCORE01.assets/image-20220729113230013.png)

![image-20220729114232203](JSCORE01.assets/image-20220729114232203.png)

![image-20220729115332342](JSCORE01.assets/image-20220729115332342.png)

![image-20220729115730961](JSCORE01.assets/image-20220729115730961.png)

## 闭包

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>闭包 14:01</title>
  </head>

  <body>
    <script>
      // 函数分两种状态:  静态 和 动态(调用)

      // 作用域链: 当出现多层作用域嵌套的场景, 如果当前作用域中没有使用的变量, 则到上层查找 -- 就近原则. 优先使用离得最近的
      var uname = "涛涛";

      function show() {
        // 局部作用域: 函数在调用时`临时`生成的对象. 函数运行结束后会销毁, 达到节省内存的目的
        var uname = "泡泡";

        // 作者的设计: 如果一个函数作用域的变量, 例如uname 在另外一个函数中被使用, 为了确保函数能够永远正常运行, 所以作者会让 这个b函数 把用到的变量 uname 所在的作用域保存起来, 防止其释放
        // scopes: 作用域们 -- 是函数自带的一个属性, 其中会保存函数用到的来自于 外部作用域的变量 所在的作用域
        // closure: 闭包.  -- 用于形容 这些被函数保存起来的 函数作用域
        var b = function () {
          console.log(uname);
        };
        // 打印操作有多种: log-输出的结果是美化后的
        // console.log(b);
        // dir: direct直接打印函数的本体 -- 是个对象类型
        console.dir(b);

        // b()
        return b; // show函数调用后的结果
      }

      var b = show();
      b(); //问: show函数已经执行完毕, 这个b函数还能打印出uname吗?
    </script>
  </body>
</html>
```

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>闭包 14:37</title>
  </head>

  <body>
    <!-- 
    闭包: 是函数的被动技能, 为了保障函数永远都能成功运行, 所以把其他的函数作用域保存在自身的scopes 里

    为什么要知道闭包概念?
    1. 面试必考概念 -- JS底层的经典设计之一
    2. 利用闭包机制 来解决全局变量污染的问题/为函数制作私有的变量 
   -->

    <script>
      (function () {
        var a = 10;
        var b = 20;

        function x() {
          var b = 30; //因为就近原则, 所以用这个b
          var c = 40;

          function y() {
            var d = 50;

            // 函数scopes属性: 存储 `使用到的` `来自其他作用域`的变量 所在的作用域 -- 为什么? 防止其他作用域自动销毁
            function z() {
              var e = 60;
              // 排除e: e是自己内部的
              console.log(a, b, c, d, e);
            }
            console.dir(z); // 猜一猜 z函数的scopes里存了什么?
          }
          y();
        }
        x();
      })();
    </script>
  </body>
</html>
```

## 作用域链

![image-20220729141114454](JSCORE01.assets/image-20220729141114454.png)

## 闭包应用-私有属性

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>函数的私有属性 15:10</title>
  </head>

  <body>
    <script>
      // 私有: 只能自己用 不让别人用
      (function () {
        // 希望这个变量 为 pao_eat 方法私有的, 存储在这个函数内不给别人用
        // 1. 把 pao_money 在一个函数作用域中声明, 不放在公共区域 -- 用匿名函数快速制作一个私有的作用域
        var pao_eat = (function () {
          var pao_money = 1000;
          // 现在: pao_eat 和 pao_money 在一起, 可以使用
          // 如果希望在 匿名函数外部 使用 pao_eat 函数
          // 通过return 把函数暴露到外部
          var pao_eat = function () {
            pao_money -= 50;
            console.log("吃饭中.., 剩余金额:", pao_money);
          };
          return pao_eat;
        })();

        pao_eat();
        pao_eat();

        function tao_eat() {
          pao_money -= 100;
          console.log("涛哥用泡泡的钱吃:", pao_money);
        }
        tao_eat();
        tao_eat();
      })();
    </script>
  </body>
</html>
```

### 练习

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>私有练习 15:31</title>
  </head>

  <body>
    <script>
      // 不让num共有, 所以放在局部作用域
      // 最快创建局部作用域的方式就是: 匿名函数
      var a = (function () {
        var num = 1;

        //必须通过返回操作, 把这个函数暴露到外部使用
        // var a = 5;  return a;
        // 等价与 return 5
        return function () {
          num++;
          console.log("num:", num);
        };
        // return a
      })();

      // dir: 是 direct -直接 的单词缩写
      console.dir(a); //查看其scopes属性

      a();
      a();
      a();

      // 模仿: 给b函数也制作一个私有的属性 num, 初始值100
      var b = (function () {
        var num = 100;
        return function () {
          num++;
          console.log("num:", num);
        };
      })();

      b();
      b();

      // 练习: 改造成 c 私有的 num
      var c = (function () {
        var num = 1000;
        return function () {
          num--;
          console.log("num: ", num);
        };
      })();

      c();
      c();
    </script>
  </body>
</html>
```

## 函数的参数复习

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>函数的参数 16:12</title>
  </head>

  <body>
    <h1 id="time"></h1>

    <script>
      // 函数: 是最基本的封装方式, 目的是复用代码
      // 封装: 把一些零散的东西装在一起, 封箱.  形成一个整体
      // 复用: 重复使用

      // 函数根据形参的个数会有多种写法

      // 具体表现如下: 把一大堆代码放在{}中, 形成一个整体, 然后起一个名字 -- 函数名 showDate.  以后通过函数名来调用{}中的代码
      // 封到一起 重复使用 -- 封装 + 复用

      // 获取当前的日期
      function showDate() {
        var now = new Date();
        var hour = now.getHours(); //时
        var minute = now.getMinutes(); //分
        var second = now.getSeconds(); //秒

        // 模板字符串: 用 反引号 `` 包围
        return `${hour}:${minute}:${second}`;
      }

      // 定时器: 定时触发...
      // 参数2: 定时的时间间隔, 单位毫秒  1000毫秒 = 1秒
      // 参数1: 一个函数, 每隔参数2的时间会自动触发
      setInterval(() => {
        // 变量d 存储的是 showDate函数 return 出来的值
        var d = showDate();
        console.log("d:", d);

        time.innerHTML = d;
      }, 1000);

      // 制作一个 abs 函数, 返回参数的 绝对值 - 正数
      // ()中书写的是 形参 -- 形容一下接收的值是什么
      function abs(num) {
        // 如果>0 就是正数, 返回num自身
        // 如果不>0 就是负数, 把 num变正数再返回
        return num > 0 ? num : -num;
        // if (num > 0) {
        //   return num
        // } else {
        //   return -num //负负得正
        // }
      }

      console.log(abs(10)); //10
      console.log(abs(-10)); //10

      // 多参数: 计算任意两个数字之和
      // 多个参数, 采用逗号进行间隔
      function add(x, y) {
        return x + y;
      }

      console.log(add(10, 20));
    </script>
  </body>
</html>
```

## arguments

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>arguments 16:43</title>
  </head>

  <body>
    <!-- arguments: 函数中隐式自带的变量. 存储函数在被调用时, 收到的所有实参 -->
    <!-- 适合的场景: 配合实现那些参数数量不固定的函数 -->

    <script>
      // 制作一个函数 add , 能够计算出任意数量个参数的总和
      function add() {
        // 作者为了应对 不固定数量传参 的场景, 为函数提供了一个隐藏的变量 arguments, 其中存储了收到的所有实参
        console.log("arguments:", arguments);

        var sum = 0; // 准备变量, 用于累加值
        for (var i = 0; i < arguments.length; i++) {
          // 下标取值, 累加到 sum中
          sum += arguments[i];
        }
        return sum; //返回累加后的总和
      }

      // 使用时:
      console.log(add(10, 20));
      console.log(add(10, 20, 44, 55));
      console.log(add(10, 20, 223, 34, 45, 65));
    </script>
  </body>
</html>
```

## 函数重载

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>函数重载技巧 17:13</title>
  </head>

  <body>
    <script>
      // 函数重载技巧: 可以让函数功能增强 -- 变身成多功能函数
      // 具体实现: 通过判断函数的 实参 个数 或 类型, 在内部执行不同的代码逻辑 -- 最终, 一个函数多种用途

      // 例如: 制作一个计算双11 商品折扣价格的函数
      // 原理: 利用if判断参数的 个数或类型 来载入不同的逻辑
      function zhekou(money) {
        // arguments: 保存了函数触发时收到的所有实参
        // 判定: 如果参数有3个 就是满减
        if (arguments.length == 3) {
          console.log("长度为3, 识别为满减操作:", arguments);
          var man = arguments[1];
          var jian = arguments[2];
          if (money >= man) {
            return money - jian;
          } else {
            return money;
          }
        }

        // 如果两个参数
        if (arguments.length == 2) {
          // 读取参数2, 识别其数据类型, 判定操作的逻辑
          var x = arguments[1];

          if (typeof x == "number") {
            console.log("识别到数字, 进入折扣模式:", arguments);
            return money * x;
          }

          if (typeof x == "string") {
            console.log("识别到字符串, 进入vip模式:", arguments);
            // 如果if的{}里只有一行代码, {}可以省略
            if (x == "vip1") {
              return money * 0.8;
            }

            if (x == "vip2") return money * 0.55;
          }
        }
      }

      // 希望使用时的效果： 消费3000元
      console.log(zhekou(3000, 0.7)); //7折价格: 2100
      console.log(zhekou(3000, 0.65)); //65折: xxxx
      console.log(zhekou(3000, "vip1")); //8折
      console.log(zhekou(3000, "vip2")); //55折
      console.log(zhekou(3000, 2000, 500)); //满2000 减500
      console.log(zhekou(3000, 2800, 700)); //满2800 减700
    </script>
  </body>
</html>
```

## 访问器语法

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>对象的访问器语法 17:46</title>
  </head>

  <body>
    <script>
      var a = { bb: "BBB", kk: "KKK" };

      var bb = "kk";
      // 点语法:  对象.属性名    属性名 写什么是什么
      console.log(a.bb);
      // 方括号语法:  对象[JS代码]

      // bb是变量,会替换为实际存储的值, bb -> 'kk';  a.kk
      console.log(a[bb]);
      console.log(a["bb"]); // 相当于 a.bb
    </script>
  </body>
</html>
```

## 总结

- 声明操作 -- ES6 版本之前
  - var - 声明变量 存储任意类型的数据
  - function - 声明函数, 只能存函数
- 作用域: 一个特殊功能的对象
  - 全局: 浏览器作为宿主环境时, 全局对象就是 window 变量
    - 宿主环境: JS 运行时所在的环境
    - window 对象:存储了浏览器提供的所有的 API 官方给的东西
  - 局部: 函数运行时临时生成的对象, 独立于全局之外
    - 需要用断点调试功能 来查看
- 怎么解决全局变量污染:
  - 用`匿名函数`自调用的方式, 制作一个函数作用域, 在这个作用域中编写代码
- 声明提升

  - function: 提升整体
  - var : 只提升声明, 不提升赋值!

- 闭包:Closure

  - 属于函数的一个`被动技能`

  - 函数中使用的变量如果来自`其他的函数作用域`, 为了防止作用域的销毁而导致变量销毁. 所以 把这些作用域保存在自身的 `scopes`属性里

    而这些被保存到 scopes 属性里的函数作用域 -- 称为闭包 (用于描述这种角色)

- 利用闭包机制能做什么?

  - 面试几乎必考

  - 为函数制作私有的变量, 格式固定

    ```js
    var 函数名 = (function () {
      var 变量 = xx;
      return function () {};
    })();
    ```

- arguments

  - 函数自带的一个 隐藏的变量. 其中保存函数触发时, 收到的所有实参
  - 函数重载技巧
    - 适合制作多功能函数
    - 利用 if 判断 参数的个数 或 类型不同, 执行不同的逻辑

> 周末时间 一定要把 `成亮`老师讲解的 JS 基础 复习一遍

## 作业

### 猜测下方代码的运行结果

```js
  <script>
    var a = 10

    function b() {
      a = 20
      console.log(a);
    }
    b()

    console.log(a);
  </script>
```

```js
  <script>
    var a = 10

    function b() {
      var a
      a = 20
      console.log(a) //20
    }

    b()
    console.log(a);
  </script>
```

```js
  <script>
    var a = 10

    function b() {
      a = 20
      console.log(a);
      var a
    }

    b()
    console.log(a);
  </script>
```

### 函数重载练习

制作一个函数, 完成如下需求

- sum(100) : 返回 1 累加到 100 的总和
- sum(50, 100): 返回 50 累加到 100 的总和
- sum(50, 100, 2) : 返回 50 52 54 ... 98 100 累加的总和, 数字间隔 2

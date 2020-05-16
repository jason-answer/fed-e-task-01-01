> Part 1. JavaScript 深度剖析
> Mod 1. ES 新特性与 JS 异步编程、TypeScript

#### 一、简答题

#### 1. 请说出下列最终的执行结果，并解释为什么？

```js
var a = []

for (var i = 0; i < 100; i++) {
  a[i] = function () {
    console.log(i)
  }
}

a[6]()
```

**答案**

​ **执行结果** `100`

​ **原因**

---

#### 2. 请说出下列最终的执行结果，并解释为什么？

```js
var temp = 123

if (true) {
  console.log(temp)
  let temp
}
```

**答案**

​ **执行结果** `Uncaught ReferenceError: Cannot access 'temp' before initialization`

​ **原因**

---

#### 3. 结合 ES6 新语法，用最简单的方式找出数组中的最小值

```js
var arr = [12, 34, 32, 89, 4]
```

**答案**

```js
arr.sort((a, b) => a - b)[0]
```

---

#### 4. 请详细说明 var，let，const 三种声明变量的方式之间的具体差别？

**答案**

---

#### 5. 请说出下列代码最终输出的结果，并解释为什么？

```js
var a = 10
var obj = {
  a: 20,
  fn() {
    setTimeout(() => {
      console.log(this.a)
    })
  },
}

obj.fn()
```

**答案**

---

#### 6. 简述 `Symbol` 类型的用途？

**答案**

---

#### 7. 说说什么是浅拷贝，什么是深拷贝？

**答案**

---

#### 8. 谈谈你是如何理解 JS 异步编程的，Event Loop 是做什么的，什么是宏任务，什么是微任务？

**答案**

---

#### 9. 将下列异步代码使用 Promsie 改进？

```js
setTimeout(function () {
  var a = 'hello'
  setTimeout(function () {
    var b = 'lagou'
    setTimeout(function () {
      var c = 'I 💕️ U'
      console.log(a + b + c)
    }, 10)
  }, 10)
}, 10)
```

---

#### 10. 请简述 TypeScript 与 JavaScript 之间的关系？

---

#### 11. 请谈谈你所认为的 TypeScript 优缺点？

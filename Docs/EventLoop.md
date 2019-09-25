### 事件循环

```javascript
new Promise(resolve => {
    resolve(1);
    Promise.resolve().then(() => console.log(2));
    console.log(4)
}).then(t => console.log(t));
console.log(3);
```

Javascript的特点就是单线程，同一时间就只做一件事。为了协调事件、用户交互、脚本、UI 渲染和网络处理等行为，防止主线程的不阻塞，Event Loop 的方案应用而生。

事件循环是通过任务队列的机制来进行协调的。每次循环称为tick



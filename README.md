# jigsaw
canvas滑动验证码

## [演示地址](https://yeild.github.io/jigsaw/demo.html)

### 用法：
1. 引入[jigsaw.min.js](https://raw.githubusercontent.com/yeild/jigsaw/master/dist/jigsaw.min.js)

2.
```
// 新增 init 方法返回一个实例,方便调用 reset 等方法
let instance = jigsaw.init({
  el: document.getElementById('container'),
  width: 310, // 可选, 默认310
  height: 155, // 可选, 默认155,
  images:[], // 新增自定义图片数组,如 ["/images/path/you/image.jpg',"/images/path/you/image-1.jpg",......]
  onSuccess: function () { ... },
  onFail: function () { ... },
  onRefresh: function () { ... }
})

// 重置验证器
instance.reset()
```

### Tips：
.
1. 图片从 https://picsum.photos/ 随机获取，然后用canvas裁剪生成滑块.

2. 支持移动端和IE浏览器(IE10+).

3. 纯前端验证不能保证安全性，本项目仅供学习交流.

# 前端复习资料
## 基础知识
```
1. 类数组转化为数组的方式
2. map,reduce,filter,every,some // 能手写实现 //循环不可停止
3. Object.create 创建一个对象与普通对象的区别
    Object.keys
    Object.value
    Object.entries,等常见的函数
4. 循环与迭代器 Iterable for of 
5. promise 的实现 promise 中用了什么设计模式 
    pormise.all 实现
    promise.race 实现
6. 编写co库模拟实现generate yeild 函数 
 实现：https://github.com/zhangjihu0/Promise_Study/tree/master/src
    循环中能使用 await 函数吗，为什么
7. http 缓存方式 强制缓存，对比缓存指的是什么 
8. 浏览器缓存 cookie sessionStorage localoStorage IndexDB 区别应用场景 前端业务方案，开源方案
9. http 0.9 1.0 2.0 https的了解 浏览器并发条数限制 2.0的保持链接通道 
    常见的状态码的含义
10. 浏览器是如何加载并解析页面的
11. 闭包的定义
    当一个函数在运行时会形成一个封闭的作用域，使内部变量不受外界影响。
    闭包的作用 保存 与 保护
12. 跨域 形成的原因与解决方案
    前端的运行环境与后端服务协议域名端口号统一否则会出现跨域
    jsonp 是什么
    后端设置请求头，白名单
    利用webpack的node能力做代理，server中配置
13. 重回与重排
```
## 应用库 
### react 
#### react 
```
心智模型 https://react.iamkasong.com/#%E7%AB%A0%E8%8A%82%E8%AF%B4%E6%98%8E
性能优化 https://www.bilibili.com/video/BV1Yr4y1J7oc/?spm_id_from=333.999.0.0&vd_source=9543ca4dbc1528c32f073539c584dd50
手写react https://www.bilibili.com/video/BV1dK411N7gp/?spm_id_from=333.337.search-card.all.click&vd_source=9543ca4dbc1528c32f073539c584dd50
手写 react hook https://www.bilibili.com/video/BV1ed4y1A74J/?spm_id_from=333.337.search-card.all.click&vd_source=9543ca4dbc1528c32f073539c584dd50
redux 用法与实现 https://www.ruanyifeng.com/blog/2016/09/redux_tutorial_part_one_basic_usages.html
手写 mobx https://www.bilibili.com/video/BV1Se4y1U7jh/?spm_id_from=333.337.search-card.all.click&vd_source=9543ca4dbc1528c32f073539c584dd50
手写 rc-form https://www.bilibili.com/video/BV1Cr4y1w7JF/?spm_id_from=333.337.search-card.all.click&vd_source=9543ca4dbc1528c32f073539c584dd50

```
#### 实现一个简单的react class hook 两版本
```

    React.createElement
    react 事件机制
    react diff 如何对比的key的作用
    react setState 同步与异步更新

    hook双缓存机制
    react hook 为了解决那两大问题
    代数效应
    定时器中如何打印出正确的state hook的声明为何只能写在组件的作用下，不能是里边的函数作用域
    react 更新是同步的还是异步的 关键帧在优化中的使用


```

#### 类实现的与hook实现的常见api 类实现时期react面临的问题，如何解决的，为什么用hook模式 
#### react 周边生态  *表示要能实现过一个类似的小型库，能聊明白原理
```
    1. redux * redux 中间的实现 异步中间件 redux-thunk(插件里我们在用) redux-sage   
    2. mobx *
    3. react-dnd *
    4. react-router *
    5. axios与fetch的对比  *
    6. rc-form 与 formily 区别 *
    7. antd  如何实现一个基本的table 
    8. umi *
    9. ahook 了解
```
## 工程化
### webpack 
```
    1. 的核心实现
    2. tapable
    3. webpack 的常见的loader与plugin的职能与使用 基本的loader与plugin 的实现原理
    例如 
        1. cssloader 
        2. style-loader  
        3. html注入插件，
        4. shadom dom 
        5. import是如何实现的 
        6. 动态引入是如何实现的
    4. 自己编写loader与插件解决实际问题 
    5. 对ast的了解
    6. babel 的配置
    7. css预处理 sess less 已解解析器
    8. css的后置处理 postCss 与常见的插件
    9. 优化方案  dll，等等有很多
```
#### cli 如何利用cli 优化公司的 开发使用体验，模板的更新，提供的助手能力等等
#### gitLab ci/cd 

#### 微前端
```
    1. single-spa 核心实现 *
    2. qiankun 核心实现 实际遇到的问题  
        沙箱  
            js 是如何实现的 
            css 沙箱有哪几种，有什么缺点
            无痛接入是如何实现的
    3. webpack 的模块联邦机制
    4. 其他的实现方式 目前市场的解决方案是什么，适合的场景是什么
```

### 微信小程序
```
如何实现的 webComponent 桥接 h5-plus
跨端解决方案有哪些  uniapp trao 
核心实现原理是什么，有什么不同，你如何做选择
```

### 我们的项目架构是什么，为了解决什么问题。为了解决这些问题大的模块的核心是什么，怎么串联这些模块





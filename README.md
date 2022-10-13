# zhaoxin-jiaotang
因为招新时间仓促，没有把三个页面做到一起，海涵海涵。

### 任务一

​	**自我介绍页面** 附有页面地址可以直接访问

### 任务二

​    1.轮播图单独完成页面在index1

​	2.发送博客展开搜索界面

​	3.评论区板块页面

​	4.更改页面主题 页面

问题1：
1.时间格式化
解决方案 ：
    引入Moment.js库使用
2.按日期排序
    存储发布日期为数组形式进行比较
    默认发布内容为日期排序
3.展开和预览
    有一个版面主要用来写标题
    另一个版面是内容（默认隐藏）
    点击展开即可展示
4.删除操作
    对应的博客赋给一个固有属性id 用于确定选择或者点中那个博客
5.剩余操作
    刚好对应的就是发布博客的操作

6.本地存储：
    本地存储为字符串格式
    

```
let data = [{
        title: 'sh',
        id: 0
    },{
        title: 'hua',
        id:12
    }
    ];
```

​    先把对象形式转为JSON字符串形式
​    JSON.stringgify(obj)
​    localStrage.setItem('data1',JSON.stringgify(obj))
​    取出时是要再从字符串格式转换为对象格式
​    let data1 = JSON.parse(localStorage.getItem('data1'));
​    这里的data1是数组对象，即可取出对应的内容啦

提示：
    自我介绍附有页面地址 可以直接访问 [Document (graceful-llama-411f55.netlify.app)](https://graceful-llama-411f55.netlify.app/)
    Index1 对应的是轮播图 
    index3 对应的是学习记录展示区

### 扩展部分

​	**1.node.js 与浏览器运行环境的取别**

​		首先全局this指向不同，一个是指向windows ,另一个是指向global(global属于windows一部分，属于浏览器定义的内置对象，一些全局属性和方法都是属于它的)

​		再有就是我们设计前端页面时可能会出现，因为浏览器引擎的不同而出现偏差，但node.js是基于谷歌V8 引擎的所以不存在这样的问题

​		再有就是浏览器通过dom操作来完成与页面的互动，但Node.js没有前台任务页面所以没有dom操作

​		 最后就是模块标准不同一个是CommonJs 标准 一个是ES模块标准

​	**2.使用一些boostrap框架 Jquery插件组 来重新搭建项目**
    **我希望附上我的银杏果项目页面设计能够为我笔试加分**

​	这里我选择用我的银杏果项目页面设计案例来答复

问题1：什么是CDN：内容分发式网络

​		资源分布在用户集中地，当大量用户向网站访问资源时，资源由集中地的本地服务器提供，而非全部由源服务器提供，降低访问堵塞。
    





​	
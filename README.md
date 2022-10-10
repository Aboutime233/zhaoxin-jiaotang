# zhaoxin-jiaotang
**本地存储：**
    本地存储为字符串格式
    `le`t data = [{`
        `title: 'sh',`
        `id: 0`
    `},{`
        `title: 'hua',`
        `id:12`
    `}`
    ];`
    先把对象形式转为JSON字符串形式
    `JS`ON.stringgify(obj)`
    localStrage.setItem('data1',JSON.stringgify(obj))`
    取出时是要再从字符串格式转换为对象格式
    let data1 = JSON.parse(localStorage.getItem('data1'));
    这里的data1是数组对象，即可取出对应的内容啦

**任务一：**
    轮播图单独完成

**任务二：**

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
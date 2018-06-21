## vue第一天复习
- vm => viewModel 数据最终都会被vm所代理。
- {{a}} 取值表达式，通过{{}}来进行取值,默认可以不写this，表达式 赋值运算 计算 三元表达式
尽量少写逻辑（computed）

### 指令：
- dom元素的行间属性，vue提供了内置的指令，必须v-开头，后面的值均为变量
    - v-model (表单元素) 忽略掉value,checked,selected,将数据绑定的视图上，视图修改后会影响数据的变化
    - v-text 取代{{}} v-cloak 解决闪烁（块）问题,后期都可以不采用，使用v-cloak要加样式
    - v-once 绑定一次，数据在变化不会导致视图刷新，写在不想刷新的标签上
    - v-html 将html字符串转化成html
    - v-for 循环(数组，对象，字符串，数字)
        ```
            <div v-for="value in/of 数组"></div>
            <div v-for="(value,index) in/of 数组"></div>
        ```
### 事件v-on(@)
- 绑定给dom元素，函数需要定义在methods中，不能和data里的内容重名，this指向的是实例，不能使用箭头函数，事件源对象如果不写括号，可以自动传入，否则只能手动传入$event
```
<div @事件名="fn"></div>
```

## 安装
```
npm install vue axios bootstrap
```




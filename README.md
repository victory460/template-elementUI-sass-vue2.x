
### template-elementUi-sass-vue2说明
- 组件封装原则，尽量扁平化，一对多，而不要层级太多、嵌套太多
- 1、router路由 根据 pages页面来配
- 2、结构组件structures（纯html,css结构，不含js）
```
pages页面中相似的结构抽出来 放在structures结构中，structures中在会变化的部分写上slot插槽

main等含有子路由的页面，引入structures后，在插槽中插入router-view

内页，引入structures后，直接在插槽中插入不同的html标签
```
- 3、功能组件components（html,css,js）把相似结构，相似功能的部分抽出来，不同的dom结构用插槽预留
```
一般在内页使用
```
- config-index.js 设置proxyTable请求代理
- components 功能组件
- config 常用参数
- eventBus 事件总线
- filters 全局过滤器
- http-http 封装的axios请求+请求loading+状态提示
- http-urls 封装的所有接口地址
- pages 页面组件
- router 路由集成表
- structures 结构组件
- utils 全局函数
- vuex 状态管理集成
- main.js 入口函数
---
# vue-cli脚手架
# itservicecenter

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

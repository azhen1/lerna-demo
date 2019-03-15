### 项目介绍
shoppingmall

二维火商家管理系统（商圈项目的管理后台）

### 项目搭建
![vue](https://img.shields.io/badge/vue-v2.5.21-green.svg)
![vuex](https://img.shields.io/badge/vuex-v3.0.1-brightgreen.svg)
![vue-router](https://img.shields.io/badge/vue_router-v3.0.2-brightgreen.svg)
![iview](https://img.shields.io/badge/iview-v2.14.3-blue.svg)
![webpack](https://img.shields.io/badge/webpack-v3.12.0-blue.svg)
![node](https://img.shields.io/badge/node-v10.12.0-green.svg)

基于vue开发的单页面应用
[vue](https://cn.vuejs.org/v2/guide/) + [vue-router](https://router.vuejs.org/zh/) + [vuex](https://vuex.vuejs.org/)

基于vue.js的开源UI组件库[iview](https://www.iviewui.com/docs/guide/install)


### 项目结构

```
.
├── build                               // 全局公共配置
├── config                              // 开发环境生产环境配置
├── page
│   └── index.html
├── src
│   ├── api                             // 项目接口
|   ├── base
│   │   ├──config                       // 接口环境配置
│   ├── components                      // 全局公共组件
│   ├── constants                       // 全局定义的枚举类型
│   ├── filters                         // 常用的公共过滤函数
│   ├── mixins
│   ├── store                           // 全局store
│   ├── util                            // 全局公共util文件夹
│   └── views                           // 页面目录
│       └── index
│           ├── agmManagement           // 补充协议管理
│           ├── basicData               // 基础参数
│           ├── cssSheet                // 联营结算单
│           ├── ctManagement            // 合同管理
│           ├── home                    // 商场首页
│           ├── mnangeMent              // 招商管理
│           ├── myDesk                  // 我的工作台
│           ├── prtManagement           // 物业管理
│           ├── salesManagement         // 销售管理
│           ├── slSheet                 // 租赁结算单
│           ├── app.vue                 // 项目主页面
│           ├── main.js                 // 入口文件
│           ├── router.js               // 路由配置
│           └── uploadTemplate.vue
├── static
├── style
├── template
├── theme
├── tmp
└── package.json

```

#### build

以下是构建时提供的别名（'alias'），用以快速引入
- `@`: 指向`/src`目录
- `static`: 静态文件目录
- `apiConfig`: 指向`src/base/config/`目录，环境信息(指项目、预发、线上等环境)
  
原则上过多的使用`alias`降低构建效率，慎重使用

#### src

主要的业务代码说明
- views/index下的每一个文件夹对应左侧导航的一个功能，该文件夹里包含的都是项目的view层
- store 是整个项目的数据层，对应view层里每个组件的管理状态
- api 所有的接口请求都被封装在该目录下

数据层
- 数据层使用vuex
- 单项数据流
- 因为物理隔离的要求，单页单store

### Use

#### 申请账号 获取权限
在二维火掌柜端(APP)申请注册账号--联系@肉圆要测试包的下载地址

两种获取商家管理后台权限的方式：（第一种方式比较麻烦 还要建立合同，建议用第二种方式）

    1.火掌柜端刚申请注册的账号下注册一个店铺 并联系@肉圆把店铺加入到某个商场(例：肉圆mall0000001)

    2.直接联系@肉圆把火掌柜端申请注册的账号设置为肉圆mall0000001商场的管理员


#### 项目运行

```bash
# install dependencies
npm install

# serve with hot reload at localhost:1314
npm run dev

# build for production with minification
npm run build
```
Your application is running here: http://0.0.0.0:1314
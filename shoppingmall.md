shoppingmall项目新手文档

### 项目介绍
商圈项目的管理后台即二维火商家管理系统商城。

### 项目搭建
![vue](https://img.shields.io/badge/vue-v2.5.21-green.svg)
![vuex](https://img.shields.io/badge/vuex-v3.0.1-brightgreen.svg)
![iview](https://img.shields.io/badge/iview-v2.14.3-blue.svg)
![webpack](https://img.shields.io/badge/webpack-v3.12.0-blue.svg)
![node](https://img.shields.io/badge/node-v10.12.0-green.svg)


### 项目结构

```
.
├── build                               // 全局公共配置
├── config                              // 开发环境生产环境配置
├── page
│   └── index.html
├── src
│   ├── api                             // 项目接口 全局app入口，对应官方app.js app.json app.wxss
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
│           ├── app.vue                 // 全局项目的入口文件
│           ├── main.js                 // 入口文件的配置
│           ├── router.js               // 全局项目的路由配置
│           └── uploadTemplate.vue
├── static
├── style
├── template
├── theme
├── tmp
└── package.json

```

### 项目账号申请与运行

在二维火掌柜端(APP)申请注册账号--联系@肉圆要测试包的下载地址

两种获取商家管理后台权限的方式：（第一种方式比较麻烦 还要建立合同，建议用第二种方式）
    1.火掌柜端刚申请注册的账号下注册一个店铺 并联系@肉圆把店铺加入到某个商场(例：肉圆mall0000001)
    2.直接联系@肉圆把火掌柜端申请注册的账号设置为肉圆mall0000001商场的管理员



```bash
# install dependencies
npm install

# serve with hot reload at localhost:1314
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```
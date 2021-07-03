# DOA example

## 运行
```sh
# 安装依赖
yarn #或npm install
# 运行脚本
yarn start #或npm run start
```

## 核心依赖

- 脚手架：create-react-app，可替换umijs
- 前端组件库：Material UI，可替换antd
- 前端数据管理：mobx，可替换dvajs
- request组件：fetch，可替换umi-request

## 代码结构
```sh
src
├── Layout.js #前端全局Layout（侧边栏，顶部工具栏等）
├── Route.js #路由，url与组件绑定
├── components #已封装组件
│   ├── Graph.js #visjs网络图封装
│   └── Title.js #用Material UI封装Title组件
├── data
│   ├── SchemaList.js #mobx数据模型定义，类似dvajs中的model
│   ├── originList.json #mock表单数据
│   ├── simpleForm.json #mock简易schema表单
│   └── startdata.json #mock流程图数据
├── index.js #前端入口
├── listItems.js #侧边栏菜单内容
├── pages #全部页面
│   ├── FSList.js #FSList页面，包含demo主要内容，已注释
│   ├── Flow.js #Flow页面，包含FSList页面中的Schema表单与流程图组件绑定，未注释
│   ├── FlowList.js #暂未使用
│   ├── FormSchema.js #暂未使用
│   ├── HomePage.js #前端默认页面
│   └── NotFoundPage.js #路由无法匹配时的404页面
└── theme.js #Material UI主题自定义
```
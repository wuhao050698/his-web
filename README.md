## 简介
 HIS-云医院-前端

## 项目架构
```
├─.github         #git包文件  
├─build           #项目配置文件
├─mock            #mock.js前端随机数据生成，模拟后端请求，独立测试  
├─node_modules    #npm所有下载的包  
├─plop-templates  #基本模板  
├─public          #静态资源  
├─src             #源代码  
│  ├─api          #所有请求api  
│  ├─assets       #主题、字体等静态资源  
│  ├─components   #全局公用组件  
│  ├─directive    #全局指令  
│  ├─filters      #全局filters 过滤器、输入验证  
│  ├─icons        #所有的svg icons  
│  ├─layout       #全局页面布局layout  
│  ├─router       #路由  
│  ├─store        #全局store管理  
│  ├─styles       #全局样式  
│  ├─utils        #全局公用方法  
│  ├─vendor       #公用vendor  
│  └─views        #所有页面  
├─tests           #部分函数的测试  
├─.env.xxx                   # 环境变量配置  
├─.eslintrc.js               # eslint 配置项  
├─.babelrc                   # babel-loader 配置  
├─.travis.yml                # 自动化CI配置  
├─vue.config.js              # vue-cli 配置  
├─postcss.config.js          # postcss 配置  
└─package.json               # package.json  
```

## 后端架构
```
his-cloud-xxx-xxx
└─src
   └─main
       ├─java
       │  └─com
       │      └─neu
       │          └─his
       │              └─cloud
       │                  └─xxx
       │                      └─xxx
       │                          ├─common         //通用类
       │                          ├─component      //切面组件
       │                          ├─config         //配置文件
       │                          ├─controller     //接口
       │                          │  ├─bms
       │                          │  ├─dms
       │                          │  ├─pms
       │                          │  └─sms
       │                          ├─distribution   //请求转发
       │                          │  └─api
       │                          │      └─pc    
       │                          │          ├─bms
       │                          │          ├─dms
       │                          │          ├─pms
       │                          │          └─sms
       │                          ├─domain    
       │                          ├─dto            //自定义数据传输对象
       │                          │  ├─app
       │                          │  ├─bms
       │                          │  ├─dms
       │                          │  ├─pms
       │                          │  └─sms
       │                          ├─filter         //自定义过滤器
       │                          ├─mapper         //mybatis generator生成dao层接口
       │                          ├─dao	           //自定义dao层接口
       │                          ├─model          //实体类
       │                          ├─service        //service接口
       │                          │  └─impl        //service接口实现类
       │                          └─util           //自定义工具类
       └─resources
           └─com
               └─neu
                   └─his
                       └─cloud
                           ├─xxx
                               ├─xxx
                                   └─mapper        //数据库映射XML

```

```
├─common      
├─components   # general purpose module
│  ├─uni-badge
│  ├─uni-card
│  ├─uni-grid
│  ├─uni-icon
│  ├─uni-list
│  ├─uni-list-item
│  ├─uni-nav-bar
│  ├─uni-rate
│  └─uni-tag
├─hybrid             # Directory for local web pages
│  └─html
├─pages              #Directory where the business page files are stored
│  └─his
│        ├─detail.vue
│        ├─doctordetail.vue
│        ├─doctors.vue
│        ├─index.vue
│        ├─inspectionResult.vue
│        ├─record.vue
│        ├─login.vue
│        ├─registrationResult.vue
│        ├─reserve.vue
├─platforms	#stors pages for each platform
├─static		#Stores  the application references static resources (such as images, videos, etc.). 
│  ├─app-plus
│  └─img
├─store		#Global store management
├─main.js                #Vue initializes the entry file
├─App.vue              #Application configuration, configures App global styles and listen to application lifecycle
├─manifest.json      #Configure App global styles and listen to Application lifecycle
├─pages.json          #Configure page routing, navigation bars, tabs, and other page class information
├─unpackage         #Uni - app can Package project as native App, wx applets, H5
└─wxcomponents  #Directory where small program components are stored
    └─vant
        ├─button
        ├─common
        │  └─style
        │      └─mixins
        ├─loading
        ├─mixins
        │  └─observer
        └─wxs
```

## 涉及的框架
  ES2015+、vue、vuex、vue-router 、vue-cli 、axios 、element-ui 、mock.js等

## 功能简介

```
- 登录 / 注销

- 权限验证
  - 页面权限
  - 指令权限
  - 权限配置
  - 二步登录

- 多环境发布
  - dev sit stage prod

- 全局功能
  - 国际化多语言
  - 多种动态换肤
  - 动态侧边栏（支持多级路由嵌套）
  - 动态面包屑
  - 快捷导航(标签页)
  - Svg Sprite 图标
  - 本地/后端 mock 数据
  - Screenfull全屏
  - 自适应收缩侧边栏

- Excel
  - 导出excel
  - 导入excel
  - 前端可视化excel
  - 导出zip

- 表格
  - 动态表格
  - 拖拽表格
  - 内联编辑

- 错误页面
  - 401
  - 404

- 組件
  - 头像上传
  - 返回顶部
  - 拖拽Dialog
  - 拖拽Select
  - 拖拽看板
  - 列表拖拽
  - SplitPane
  - Dropzone
  - Sticky
  - CountTo

- 错误日志
- Dashboard
- 引导页
- ECharts 图表
- Clipboard(剪贴复制)
```

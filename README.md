# mall-app-web
<p>
  <a href="https://github.com/ChangSZ/mall"><img src="./images/后台项目-mall-blue.svg" alt="后台项目"></a>
  <a href="https://github.com/ChangSZ/mall-admin-web"><img src="./images/前端项目-mall--admin--web-green.svg" alt="前端项目"></a>
</p>

## 前言

该项目为前后端分离项目的前端部分，后端项目`mall`地址：[传送门](https://github.com/ChangSZ/mall-go)。

## 项目介绍

`mall-app-web`是一个电商系统的移动端项目，基于`uni-app`实现。主要包括首页门户、商品推荐、商品搜索、商品展示、购物车、订单流程、会员中心、客户服务、帮助中心等功能。

### 项目演示

项目在线演示地址：[http://mall.water-melon.top/app/](http://mall.water-melon.top/app/)  

### 效果展示

![](./images/mall_app_web_preview_01.png)![](./images/mall_app_web_preview_02.png)

![](./images/mall_app_web_preview_03.png)![](./images/mall_app_web_preview_04.png)

![](./images/mall_app_web_preview_05.png)![](./images/mall_app_web_preview_06.png)

![](./images/mall_app_web_preview_07.png)![](./images/mall_app_web_preview_08.png)

![](./images/mall_app_web_preview_09.png)![](./images/mall_app_web_preview_10.png)



### 技术选型

| 技术         | 说明             | 官网                                    |
| ------------ | ---------------- | --------------------------------------- |
| Vue          | 核心前端框架     | https://vuejs.org                       |
| Vuex         | 全局状态管理框架 | https://vuex.vuejs.org                  |
| uni-app      | 移动端前端框架   | https://uniapp.dcloud.io                |
| mix-mall     | 电商项目模板     | https://ext.dcloud.net.cn/plugin?id=200 |
| luch-request | HTTP请求框架     | https://github.com/lei-mu/luch-request  |

### 项目结构

``` lua
src -- 源码目录
├── api -- luch-request网络请求定义
├── components -- 通用组件封装
├── js_sdk -- 第三方sdk源码
├── static -- 图片等静态资源
├── store -- vuex的状态管理
├── utils -- 工具类
└── pages -- 前端页面
    ├── address -- 地址管理页
    ├── brand -- 商品品牌页
    ├── cart -- 购物车页
    ├── category -- 商品分类页
    ├── coupon -- 优惠券页
    ├── index -- 首页
    ├── money -- 支付页
    ├── notice -- 通知页
    ├── order -- 订单页
    ├── product -- 商品页
    ├── public -- 登录页
    ├── set -- 设置页
    ├── user -- 会员页
    └── userinfo -- 会员信息页
```

## 搭建步骤

- 本项目使用了`uni-app`专用开发工具`HBuilder X`（App开发版）开发，下载地址：https://www.dcloud.io/hbuilderx.html
- 该项目为前后端分离项目，访问本地访问接口需搭建后台环境，搭建请参考后端项目[传送门](https://github.com/ChangSZ/mall)；
- 注意由于`mall-app-web`中的接口都在`mall-portal`模块中，所以一定要启动该模块；
- 访问在线接口无需搭建后台环境，只需将`utils/appConfig.js`文件中的`API_BASE_URL`改为线上地址即可：`http://mall-portal.water-melon.top`
- 克隆源代码到本地，使用`HBuilder X`打开；
- 在`HBuilder X`中使用`运行->运行到浏览器->Chrome`运行项目，运行成功后会自动打开下面地址（将浏览器改为手机模式）：http://localhost:8080
- 如果浏览器没有启动的话，可以直接访问如下地址访问：http://localhost:8080

## 许可证

[Apache License 2.0](https://github.com/ChangSZ/mall-app-web/blob/master/LICENSE)

Copyright (c) 2024-2024 ChangSZ
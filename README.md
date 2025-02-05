

# RuoYi AI



<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]


<!-- PROJECT LOGO -->
<br />


<img style="text-align: center;" src="image/00.png" alt="Logo" width="150" height="150">

<h3 style="text-align: center;">快速搭建属于自己的 AI 助手平台</h3>

<p style="text-align: center;">
    全新升级，开箱即用，简单高效
    <br />
    <a href="https://doc.pandarobot.chat"><strong>探索本项目的文档 »</strong></a>
    <br />
    <br />
    <a href="https://web.pandarobot.chat">项目预览</a>
    ·
    <a href="https://github.com/ageerle/ruoyi-ai/issues">报告Bug</a>
    ·
    <a href="https://github.com/ageerle/ruoyi-ai/issues">提出新特性</a>
</p>

## 目录

- [源码地址](#源码地址)
- [特色功能](#特色功能)
- [项目演示](#项目演示)
  - [后台管理](#后台管理)
  - [用户端](#用户端)
  - [小程序端](#小程序端)
- [开发前的配置要求](#开发前的配置要求)
- [文件目录说明](#文件目录说明)
- [使用到的框架](#使用到的框架)
- [贡献者](#贡献者)
  - [如何参与开源项目](#如何参与开源项目)
- [版本控制](#版本控制)
- [作者](#作者)
- [鸣谢](#鸣谢)

### 源码地址
- 前端-后台管理: https://github.com/ageerle/ruoyi-admin
- 前端-用户端: https://github.com/ageerle/ruoyi-web
- 小程序端: https://github.com/ageerle/ruoyi-uniapp
- 演示地址: https://web.pandarobot.chat
- 后台管理: https://admin.pandarobot.chat
- 用户名: admin 密码：admin123

### 特色功能
1. 内置SSE、websocket等网络协议，支持对接OpenAI、Azure、ChatGLM、讯飞星火等大语言模型
2. 支持接入个人微信或企业微信
3. 支持易支付、微信支付和Stripe国际信用卡支付
4. 提供邮箱登录和微信公众号登录
5. 支持知识库功能，支持AI翻译、AI PPT制作、语音克隆和AI翻唱
6. 提供完整的前端应用、后台管理以及小程序应用，全部开箱即用。基于MIT开源协议


### 项目演示

#### 后台管理
<div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;">
  <img src="image/02.png" alt="drawing" style="width: 600px; height: 300px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
  <img src="image/03.png" alt="drawing" style="width: 600px; height: 300px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
  <img src="image/04.png" alt="drawing" style="width: 600px; height: 300px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
  <img src="image/05.png" alt="drawing" style="width: 600px; height: 300px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
</div>


#### 用户端
<div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;">
  <img src="image/08.png" alt="drawing" style="width: 600px; height: 300px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
  <img src="image/09.png" alt="drawing" style="width: 600px; height: 300px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
  <img src="image/10.png" alt="drawing" style="width: 600px; height: 300px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
  <img src="image/11.png" alt="drawing" style="width: 600px; height: 300px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
</div>

#### 小程序端
<div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: flex-start;">
  <img src="image/06.png" alt="drawing" style="width: 320px; height: 600px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
  <img src="image/07.png" alt="drawing" style="width: 320px; height: 600px; border: 2px solid #ddd; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"/>
</div>

### 开发前的配置要求

1. jdk 17
2. mysql 5.7、8.0
3. redis 版本必须 >= 5.X
4. maven 3.8+
5. nodejs 20+ & pnpm

### 文件目录说明
RuoYi-AI

```
├─ ruoyi-admin                         // 管理模块
│  └─ RuoYiApplication                 // 启动类
│  └─ RuoYiServletInitializer          // 容器部署初始化类
│  └─ resources                        // 资源文件
│      └─ i18n/messages.properties     // 国际化配置文件
│      └─ application.yml              // 框架总配置文件
│      └─ application-dev.yml          // 开发环境配置文件
│      └─ application-prod.yml         // 生产环境配置文件
│      └─ banner.txt                   // 框架启动图标
│      └─ logback-plus.xml             // 日志配置文件
│      └─ ip2region.xdb                // IP区域地址库
├─ ruoyi-common                        // 通用模块
│  └─ ruoyi-common-bom                 // common依赖包管理
   └─ ruoyi-common-chat                // 聊天模块
│  └─ ruoyi-common-core                // 核心模块
│  └─ ruoyi-common-doc                 // 系统接口模块
│  └─ ruoyi-common-encrypt             // 数据加解密模块
│  └─ ruoyi-common-excel               // excel模块
│  └─ ruoyi-common-idempotent          // 幂等功能模块
│  └─ ruoyi-common-json                // 序列化模块
│  └─ ruoyi-common-log                 // 日志模块
│  └─ ruoyi-common-mail                // 邮件模块
│  └─ ruoyi-common-mybatis             // 数据库模块
│  └─ ruoyi-common-oss                 // oss服务模块
│  └─ ruoyi-common-pay                 // 支付模块
│  └─ ruoyi-common-ratelimiter         // 限流功能模块
│  └─ ruoyi-common-redis               // 缓存服务模块
│  └─ ruoyi-common-satoken             // satoken模块
│  └─ ruoyi-common-security            // 安全模块
│  └─ ruoyi-common-sensitive           // 脱敏模块
│  └─ ruoyi-common-sms                 // 短信模块
│  └─ ruoyi-common-sse                 // sse流推送模块（待更新）
│  └─ ruoyi-common-tenant              // 租户模块
│  └─ ruoyi-common-translation         // 通用翻译模块
│  └─ ruoyi-common-web                 // web模块
│  └─ ruoyi-common-websocket           // websocket服务集成模块（待更新）
├─ ruoyi-modules                       // 模块组
│  └─ ruoyi-demo                       // 演示模块
│  └─ ruoyi-generator                  // 代码生成模块
│  └─ ruoyi-system                     // 业务模块
├─ .run                 // 执行脚本文件
├─ .editorconfig        // 编辑器编码格式配置
├─ LICENSE              // 开源协议
├─ pom.xml              // 公共依赖
├─ README.md            // 框架说明文件


```

### 使用到的框架

- [Vben Admin](https://github.com/vbenjs/vue-vben-admin)
- [Naive UI](https://www.naiveui.com)
- [RuoYi-Vue-Plus](https://gitee.com/dromara/RuoYi-Vue-Plus)

### 贡献者

请阅读[CONTRIBUTING](https://github.com/ageerle/ruoyi-ai/graphs/contributors) 查阅为该项目做出贡献的开发者。

#### 如何参与开源项目

贡献使开源社区成为一个学习、激励和创造的绝佳场所。你所作的任何贡献都是**非常感谢**的。


1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



### 版本控制

该项目使用Git进行版本管理。您可以在repository参看当前可用版本。

### 进群学习

<div>
  <img src="image/01.png" alt="drawing" width="300px" height="300px"/>
</div>

### 版权说明

该项目签署了MIT 授权许可，详情请参阅 [LICENSE.txt](https://github.com/ageerle/ruoyi-ai/blob/master/LICENSE.txt)

### 鸣谢
- [chatgpt-java](https://github.com/Grt1228/chatgpt-java)
- [RuoYi-Vue-Plus](https://gitee.com/dromara/RuoYi-Vue-Plus)
- [chatgpt-web-midjourney-proxy](https://github.com/Dooy/chatgpt-web-midjourney-proxy)


<!-- links -->
[your-project-path]:https://github.com/ageerle/ruoyi-ai
[contributors-shield]: https://img.shields.io/github/contributors/ageerle/ruoyi-ai.svg?style=flat-square
[contributors-url]: https://github.com/ageerle/ruoyi-ai/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/ageerle/ruoyi-ai.svg?style=flat-square
[forks-url]: https://github.com/ageerle/ruoyi-ai/network/members
[stars-shield]: https://img.shields.io/github/stars/ageerle/ruoyi-ai.svg?style=flat-square
[stars-url]: https://github.com/ageerle/ruoyi-ai/stargazers
[issues-shield]: https://img.shields.io/github/issues/ageerle/ruoyi-ai.svg?style=flat-square
[issues-url]: https://img.shields.io/github/issues/ageerle/ruoyi-ai.svg
[license-shield]: https://img.shields.io/github/license/ageerle/ruoyi-ai.svg?style=flat-square
[license-url]: https://github.com/ageerle/ruoyi-ai/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555




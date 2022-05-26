# 联系我
- 手机: 18500195263
- email: fengjianok@gmail.com

---

# 关于我
- 冯建/男/1988/上海
- 专科/复旦大学(自考)
- 工作年限: 2012 ～ 至今, 11年
- Github: [https://github.com/Overu](https://github.com/Overu)
- 期望职位: JavaScript/前端工程师
- 简历: [https://github.com/Overu/resume/blob/master/resume.md](https://github.com/Overu/resume/blob/master/resume.md)

---

# 工作经历
## 上海微盟企业发展有限公司 (2020.04 ~ 2022.05)
### 智慧零售商户助手（小程序）
- 初期接手以功能迭代为主，涉及开单、商品等部分复杂的功能，很快就负责整体开发
- 因业务和需求多变，又涉及多个小程序代码共享的问题，开始着手推翻重写架构，支持模块开发、模块可拔插等，配合CLI和不同的配置文件编译出不同的小程序类型，可以针对一个业务或者多个业务打包
- 改造开发、测试流程，极大提高效率

### Kratos
- 微盟小程序平台，提供了一种用微信小程序的语法和开发方式开发微盟小程序，将小程序变成第一语言，一套代码、多端运行，支持小程序组件和Vue组件混编
- 由Android/iOS SDK、小程序转译工具和运行时、后端审核和版本管理平台组成
- 第三方开发者或有自研能力的商户可以将自己的小程序移植到微盟小程序平台，同时也支持整体部署在自有的App中
- 基于pnpm、TypeScript、Vue、vite、esbuild、swc、postCSS等，从0搭建现代化的工程体系
- 前端负责人和主程序员

### 搜狗小程序
- 搜狗输入法小程序，提供登陆、选择商户、分享商品信息到聊天框等功能
- 基于Vue、TypeScript、Webpack
- 独立开发

### base-bridge
- 封装Android/iOS bridge，提供标准化接口，为App中大量的Hybrid页面提供服务
- TypeScript
- 独立开发

## 宁波华鼐时空网络科技有限公司 (2019.06 ~ 2020.03)
### vsmap
- 3D地图渲染SDK，支持在线编辑POI样式
- 基于WebGL，自研架构，抽象Node，除了渲染节点和数据节点外，还提供了很多特殊功能的节点，比如在视角范围内自动替换渲染目标
- 独立开发
- 通过使用Web Worker处理大规模顶点数据，包括样式、顶点合并等

### triangulation
- 地图数据转换工具，用于将不同的数据源转换成[vsmap](#vsmap)能识别的私有格式，同时实现数据校验、三角化等
- Kotlin，通过KTS实现可编程的样式配置，抽象数据源，设计了中间格式，提供插件机制，打包成CLI
- 独立开发

## 上海翎阳网络科技有限公司 (2018.09 ~ 2019.06)
### Keystore
- 企业级数字货币网银SDK，包括加密算法、证书操作、通信、数据序列化、密钥存储、操作规范流程API等功能，提供对[illidan](#illidan)和[neltharion](#neltharion)的支持
- 基于C++、libuv，通过交叉编译支持[illidan](#illidan)，通过Node N-API支持[neltharion](#neltharion)
- 负责部分通信功能、证书派发和验证等功能实现
- 基于libuv实现简单的设备发现、连接，用于[illidan](#illidan)和[neltharion](#neltharion)的连接

### illidan
- 企业级数字货币签名App，为[neltharion](#neltharion)提供密钥管理、数字证书、加解密等服务
- 基于React Native、React Navigation、Dva，通过RN C++ Module包装[Keystore](#Keystore)以提供JS层API
- App负责人和主程序员，技术选型和核心代码编写
- 通过RN C++ Module的能力，屏蔽了Android/iOS底层bridge实现的差异，同时也可以直接暴露C++模块的API


项目地址: [https://enterprise.keystore.com/](https://enterprise.keystore.com/)

### neltharion
- 企业级数字货币网银，为企业数字货币资产活动提供财务流程、操作规范和有效监管，支持多币种、收付款、报表、角色权限等一系列功能
- 采用Electron、React、Mobx等，基于TypeScript，通过Electron Node N-API集成[Keystore](#Keystore)，采用更现代的工程管理体系，配合CI等工具极大得提高开发和测试效率
- 前端负责人和主程序员，前端技术选型和核心代码编写

项目地址: [https://enterprise.keystore.com/](https://enterprise.keystore.com/)

## 宁波华鼐时空网络科技有限公司 (2017.09 ~ 2018.09)
### MapCube
- JavaScriptD地图渲染SDK，支持室内外地图同屏展示，一体化定位导航，支持数据预处理
- 基于WebGL、Flow.js、Webpack等，私有数据格式
- 主程序员，基础代码编写和集成高德室外地图、转换工具等
- 通过转换工具对地图数据进行预处理，即可以避免数据暴露，同时也可以让三角化、合并等耗时操作脱离浏览器

demo: 地图数据比较大，网络较慢，需要梯子，请耐心等待。[https://overu.github.io/mapcube-example/index.html](https://overu.github.io/mapcube-example/index.html)

## 上海图聚智能科技股份有限公司 (2013.09 ~ 2017.08)
### JavaScript 3D地图渲染引擎
- JavaScript地图渲染SDK，与3D地图引擎保持一致（API、渲染效果），也是主要的产品，支持室内多楼层同屏交互渲染
- 基于three.js，同时也对WebGL进行了探索，对负担较重的计算任务（如定位算法），放到Web Worker中
- 主要负责人和主程序员，从技术选型到核心代码编写等

### Android 3D地图渲染引擎
- 3D地图渲染SDK，底层使用C/C++实现，一套代码，可以跨Android、iOS、macOS、Windows等平台运行，支持通过Lua自定义地图样式
- 基于Irrlicht，屏蔽不同平台图形API的差异，不仅可以跨平台，还支持跨引擎
- 主要负责人和主程序员，从技术选型到核心代码编写、Android端的编译
- 针对内存泄漏做了很多工作，比如包装C++对象，增加引用计数，在逃逸到Java层的时候提供计数的稳定，渲染优化，对静态POI合并，减少渲染批次

### Android 2D地图渲染引擎
- 2D地图渲染SDK，对GeoJSON数据解析渲染，提供丰富的
- 独立开发，从0到1，接触了Android 2D graphics API，对图形渲染有了初步认识，有了基本图形学的概念
- 大量优化实践，比如对POI达到一定量级的地图渲染会有卡顿的行为，需要对地图数据进行分片，每个分片交由一个线程渲染，然后主线程合成

## 上海睿泰信息科技有限公司 (2012.02 ~ 2013.08)
### 科瑞星幼教平台
- 面向幼儿的多媒体教育平台，支持分发多媒体课件资源、提供实时教学，在线多人协作，类似Google Drive
- 参考Google Wave的技术特征，通过实时编辑和冲突处理策略实现了在线多人协作
- 负责前端开发，通过使用Google Closure对组件和模块的概念有了认识，同时协助做了部分后端开发，接触了Vert.x

### 阅读器
- 基于HTLM5/CSS3的在线阅读器
- Hybrid的早期探索，使用PhoneGap(Apache Cordova)编译到不同平台，基于GWT实现Java to JavaScript的转换
- 负责前端开发
--- 

# 业余项目

### wx-compiler
将微信小程序组件(script、json、wxml、wxss)转化为Vue Component Render，支持绝大多数的语法
- 对swc、esbuild做了大量探索和应用
- wxml repl：[https://overu.github.io/wx-ast-explorer/index.html](https://overu.github.io/wx-ast-explorer/index.html)

### 单位换算
用于进行单位换算，Android App，自己的业余实践，主要为了学习和了解RoboGuice(Google Guice扩展，轻量级IoC框架)。

- 链接: [https://github.com/Overu/conversion](https://github.com/Overu/conversion)

---

# 技能
- 语言: JavaScript/TypeScript/Java/Kotlin/C/C++
- 前端框架: Vue/React/ReactNative
- 前端工具: vite/webpack/rollup
- 平台: Android/Electron/微信小程序/Hybrid
- 其他: WebGL/Node.js

-- -
# 感谢
感谢您认真阅读我的简历,因为文笔有限,总结能力也不尽人意,很多方面也会有纰漏,请多担待.如果能获得一次面试的机会,不胜感激.
# 联系我
- 手机: 18500195263
- email: fengjianok@gmail.com

---

# 关于我
- 冯建/男/1988/上海
- 专科/复旦大学(自考)
- 工作年限: 2012 ～ 至今, 9年
- Github: [https://github.com/Overu](https://github.com/Overu)
- 期望职位: JavaScript/前端工程师
- 期望薪资: 23 ~ 28k
- 简历: [https://github.com/Overu/resume/blob/master/resume.md](https://github.com/Overu/resume/blob/master/resume.md)

---

# 工作经历
## 宁波华鼐时空网络科技有限公司 (2019.06 ~ 2020.03)
### vsmap
受到之前公司的邀请.基于WebGL的高性能室3D地图渲染引擎.除了实现基本的功能外,主要的亮点在于提供用户可配置样式.用户通过编辑样式脚本文件可以配置出不同主题的样式,实现对地图中每一个POI样式高度可配置化.我独立开发,修改样式涉及到对顶点数据的大量操作,我把这些操作放到Web Worker中,顶点数据存在ArrayBuffer中,因为ArrayBuffer实现了Transferable接口,从而避免了在两个线程做大量的数据拷贝,这样不仅提高效率,还能避免内存的浪费,同时优化了文字渲染,使原来需要每个POI一个渲染批次,缩减到每一个层只需要一个.因为受到疫情影响,导致会展业务无法开展,现金流枯竭,整个研发中心被撤.

demo: [https://unimap.ai/demo/mapedit/](https://unimap.ai/demo/mapedit/)

### triangulation
用于将数据部门的生产的地图数据转换成vsmap支持的私有渲染格式,转换过程中会进行数据校验、数据优化、数据三角化,最后输出供[vsmap](#vsmap)渲染使用,代码通过Kotlin实现,最终编译成一个命令行工具.我独立开发,因为涉及到多种数据格式的转换,需要提供多个数据源和不同数据格式的支持,在设计的时候提供了数据源的抽象、中间格式和插件机制.这样我们只需要关注对数据源抽象的实现,就可以方便的将一个不同的数据格式转换成vsmap支持的格式.通过Kotlin kts,我们可以方便的外挂插件,这样可以自定义一些操作满足不同数据源定制化的要求.

## 上海翎阳网络科技有限公司 (2018.09 ~ 2019.06)
### Keystore
企业级数字货币网银SDK,包括加密算法、证书操作、通信、数据序列化、密钥存储、操作规范流程API等功能,由C++实现,同时服务[illidan](#illidan)和[neltharion](#neltharion).neltharion通过Electron提供的Node.js N-API与之集成.illidan通过RN间接提供的原生访问能力与之交互,绝大多数代码在两端共享.neltharion和illidan通过Keystore提供的通信功能连接,neltharion调用加密和数字证书的API构造发送命令,illidan接受命令同样通过验证证书和解密的API验证命令的合法性.我主要负责部分功能的实现,如证书的派生、验证,部分通信功能的实现,比如设备发现、设备连接、和Electron的libuv集成、操作规范流程API的实现、对neltharion和illidan需要的bridge代码的实现，以及两个平台的代码编译集成等.整个项目是个复杂的异构系统,能参与其中的绝大部分,对我收益良多,不仅完善了技术栈,也开拓了眼界.

### illidan
企业级数字货币签名App.扩展[neltharion](#neltharion)的功能,提供对neltharion通信、加解密、密钥存储、数字证书相关操作.将手机作为一个硬件密钥,也是每一个用户的唯一标识,用户在使用neltharion时,通过自定义的通信协议连接到硬件密钥,对所有用户的高危操作,比如付款、鉴权、审批、修改设置、重置密钥等都需要通过硬件密钥加密,最后把结果发送至服务器认证,只有通过后才会进行操作.我主要负责整个App的架构,包括架构选型、组件开发、框架封装、RN C++ Module实现、bridge代码编写,因为涉及到Android和iOS,也鉴于我们团队有React的开发经验,选用了ReactNative,路由使用React Navigation,状态管理使用dva.另外通过对RN的研究,确定了RN支持C++ Module,这样极大降低我们跨平台的成本,同时也避免了写过多的bridge代码,避免内存泄漏等导致崩溃的问题.整个架构很好的支撑了App的工作,做好了承上启下的作用.

项目地址: [https://enterprise.keystore.com/](https://enterprise.keystore.com/)

### neltharion
企业级数字货币网银,主要用于将传统企业的财务流程通过软件和一系列规范应用于企业数字货币资产中,使数字货币在企业财务环境下流通变得可以监管和控制.产品提供管理多个币种、收付款、生成财务报表、通过角色权限管理企业财务参与人员等功能.我主要负责前端架构,包括组件开发、路由框架、权限控制、状态事件等,通过TSLint编写强制了一套编码规范,因为是客户端产品,面向MacOS和Windows,我们采用Electron,UI部分使用React,状态管理用Mobx,并且衍生出适合团队的一套框架,全部的代码用TypeScript编写,还参与了整套内部CI的建设,编写了各种构建脚本.通过这个产品我涉及了前端架构方面的工作,开阔了前端技术的视野.

项目地址: [https://enterprise.keystore.com/](https://enterprise.keystore.com/)

## 宁波华鼐时空网络科技有限公司 (2017.09 ~ 2018.09)
### MapCube
完全基于WebGL的高性能室内外一体化的3D地图渲染引擎,不仅同屏可以展示室内地图,还可以展示室外的地图,提供极好的用户体验.我作为主要开发人员,集成了高德室外地图,完成了导航算法,并实现了室内外一体化无缝导航(目前高德尚未实现),定义了地图私有数据格式,并开发了配套数据转换工具.由于采用数据转换工具预处理的机制,避免浏览器进行数据三角化等CPU密集的操作,极大的提高渲染效率,即使是上万个POI也能轻松渲染.该项目出于是SDK类的产品,对性能、可靠性、健壮性都有很高的要求,我们采用了Flow.js做类型检查,避免出现因为类型问题导致的代码错误,同时也方便JS引擎对代码的优化.

demo: 网络较慢,需要梯子,请耐心等待.[https://overu.github.io/mapcube-example/index.html](https://overu.github.io/mapcube-example/index.html)

## 上海图聚智能科技股份有限公司 (2013.09 ~ 2017.08)
### JavaScript 3D地图渲染引擎
支持浏览器端的3D地图渲染引擎.基于three.js,与其他的平台的地图渲染引擎保持一致(接口、渲染效果等).我作为主要负责人,参与了技术选型、原型展示、代码编写等工作,技术栈回到了JavaScript,研究了ES6规范,使用了前端的一些常用工具,如Webpack、Babel等,也对WebGL的规范深入了解,移植了定位算法,并放在Web Worker中执行.我在公司期间开发的产品支撑起了公司大部分的项目,带了实际的收益,通过开发者平台也为外部开发者接入LBS应用提供了便利.

### Android 3D地图渲染引擎
由于2D渲染引擎无法满足市场的需求,开发了3D的地图渲染引擎.因为对跨平台有要求,需要支持Android、iOS、macOS、Windows,经过调研,决定底层使用C/C++开发,通过对图形引擎的调研,选用了Irrlicht,这样不仅对底层图形API透明,也对OS透明.我作为主要负责人,参与了前期技术选型、核心代码和Android代码的编写,通过整个项目对图形学有了深入的了解,掌握了C++,并基于C++ 11的规范编写代码,学会使用NDK编译,编写CMake脚本.同时也解决了渲染效率、内存泄漏等问题.

### Android 2D地图渲染引擎
地图渲染引擎,通过获取服务端GeoJSON数据,完成对数据的渲染,并为开发者提供接入,且提供丰富的接口进行交互.我负责所有的开发工作,开发过程中逐渐掌握了Android 2D graphics API,对图形学有了一定了解,同时也碰到了很多困难,尤其是在地图数据超过一定量级后,会有渲染丢帧的问题,经过优化,采取对地图数据分片,子线程渲染,主线程合成,进而大大提高渲染效率.提高开发者和用户的体验.

## 上海睿泰信息科技有限公司 (2012.02 ~ 2013.08)
### 科瑞星幼教平台
面向幼儿的多媒体教育平台,通过平台分发多媒体课件资源提供在线学习,并提供实时教学,教师端的操作会实时展示在学生端,类似Google Drive.前端采用Google Closure,后端是团队自研框架.我负责所有前端和部分后端工作,总结上一个项目对GWT的实践,通过GWT编译出来的JavaScript文件执行效率并不高,经过调研最终选择了Google Closure,通过对Closure的使用,对前端模块和组件有了一定的认识,自己也扩展了一些组件.同时也参与了部分后端开发工作,接触了Jersey/Vert.x等,对RESTful也有了一些了解,也了解了一些Google Wave的技术细节.

### 阅读器
基于HTLM5/CSS3的在线阅读器,使用PhoneGap(Apache Cordova)编译到不同平台,基于GWT实现Java to JavaScript的转换.我负责所有的前端工作,通过工作接触到了现代前端技术,对Hybrid有了个初步的了解,认识了代码转换技术,也解锁了Google相关技能,养成了良好的编码习惯,培养独立解决问题的能力.

--- 

# 开源项目

### 单位换算
用于进行单位换算,Android App,自己的业余实践,主要为了学习和了解RoboGuice(Google Guice扩展,轻量级IoC框架).

- 链接: [https://github.com/Overu/conversion](https://github.com/Overu/conversion)

---

# 技能
- 语言: JavaScript/TypeScript/Java/Kotlin/C/C++
- 前端框架: React/ReactNative
- 前端工具: webpack/rollup
- 平台: Android/Electron
- 其他: WebGL/Node.js

-- -
# 感谢
感谢您认真阅读我的简历,因为文笔有限,总结能力也不尽人意,很多方面也会有纰漏,请多担待.如果能获得一次面试的机会,不胜感激.
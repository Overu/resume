# Contact me
- Mobile: 18500195263
- E-mail: fengjianok@gmail.com

---

# About me
- jian.feng/Male/1988/Shanghai
- Junior College/ Fudan University (self-taught)
- Years of work: 2012 ~ present, 11 years
- Github: https://github.com/Overu
- Desired Position: JavaScript/Front-end Engineer
- Resume : https://github.com/Overu/resume/blob/master/resume.md

---

# Work Experience
## Shanghai Weimob Enterprise Development Co., Ltd. (2020.04 ~ 2022.05)
### Smart Retailer Assistant (MiniProgram)
- The initial mainly takes over the function iteration, involving some complex functions such as billing and commodities, soon responsible for the overall development.
- Due to the changeable business and requirements, and the problem of code sharing of multiple MiniPrograms, we started to overturn and rewrite architecture to support module development, module pluggable, etc., and compile different MiniProgram types with CLI and different configuration files, which can be packaged for one business or multiple businesses.
- Basing on the technology stack of MiniProgram, by using Gulp to increase the compilation layer to achieve module isolation, module life cycle, module compilation, configuration analysis and code injection, etc.
- Develop and test the process, and greatly improve the efficiency.

### Kratos
- Weimob MiniProgram platform, which provides a way to develop Weimob MiniProgram with the syntax and development method of WeChat MiniProgram, turning the MiniProgram into the first language, one set of code, multi-terminal operation, and supporting the mixing of MiniProgram components and Vue components edit
- Consists of Android/iOS SDK, MiniProgram translation tools and runtime, back-end auditing and versioning platform
- Third-party developers or merchants with self-research capabilities can port their own MiniPrograms to the Weimob MiniProgram platform, while also supporting overall deployment in their own apps
- Build a modern engineering system from scratch based on pnpm, TypeScript, Vue, vite, esbuild, swc, postCSS, etc.
- Front-end principal and Lead Programmer 

### Sogou MiniProgram
- Sogou input method MiniProgram, providing functions such as logging in, selecting merchants, sharing product information to chat boxes, etc.
- Based on Vue，TypeScript，Webpack
- Independent development

### base-bridge
- Encapsulate Android/iOS bridge, provides standardized interface to provide services for a large number of Hybrid pages in the App.
- TypeScript
- Independent development

## Ningbo Huanai Space-Time Network Technology Co., Ltd. (2017.09 ~ 2020.03)
### vsmap
- 3D map rendering SDK, support online editing POI style
- Based on WebGL, self-developed architecture, abstract Node, in addition to rendering nodes and data nodes, also provides many special functions of the node, such as automatic replacement of the rendering target in the view range
- Independent development
- Using Web Worker to process large-scale vertex data including styles, vertex merging, etc.

### triangulation
- Map data conversion tool for converting different data sources into a private format that can be recognized by [vsmap](#vsmap), and implementing data validation, triangulation, etc
- Kotlin, implements programmable style configuration through KTS, abstracts data sources, designs intermediate formats, provides plug-in mechanism, and packages into CLI
- Independent development

### Keystore
- Enterprise-level digital currency online banking SDK, including encryption algorithm, certificate operation, communication, data serialization, key storage, operation specification process API and other functions, providing support for [illidan](#illidan) and [neltharion](#neltharion) support
- Based on C++, libuv, supports [illidan](#illidan) through cross-compilation, [neltharion](#neltharion) through Node N-API
- Responsible for some communication functions, certificate distribution, verification and other functions
- Implement simple device discovery and connection based on libuv for [illidan](#illidan) and [neltharion](#neltharion)

### illidan
- An enterprise-level digital currency signature app that provides key management, digital certificates, encryption and decryption services for [neltharion](#neltharion)
- Based on React Native, React Navigation, Dva, wrapping [Keystore](#Keystore) through RN C++ Module to provide JS layer API
- App principal and lead programmer, technology selection and core code writing
- The capabilities of RN C++ Module shields the difference of Android/iOS underlying bridge implementation, and also exposes the API of C++ module directly

Project address: [https://enterprise.keystore.com/](https://enterprise.keystore.com/)


### neltharion
- Enterprise-level digital currency online banking, providing financial processes, operational specifications and effective supervision for enterprise digital currency asset activities, supporting a range of functions such as multi-currency, payment and receipt, reporting, role permissions, etc.
- Adopt Electron, React, Mobx, etc., based on TypeScript, integrate [Keystore](#Keystore) through Electron Node N-API. Adopt a more modern engineering management system, with CI and other tools, which greatly improved the development and testing efficiency
- Front-end principal and lead programmer, front-end technology selection and core code writing

Project address: [https://enterprise.keystore.com/](https://enterprise.keystore.com/)

### MapCube
- JavaScriptD map rendering SDK, support indoor and outdoor map display on the same screen, integrated positioning and navigation, support data pre-processing
- Based on WebGL, Flow.js, Webpack, etc., private data formats
- Lead programmer, basic code writing and integration of Gaode outdoor maps, conversion tools, etc.
- Preprocessing of map data through conversion tools can avoid data exposure, and at the same time, time-consuming operations such as triangulation and merging can be removed from the browser

demo: The map data is relatively large, the network is slow and a ladder is required, please be patient.[https://overu.github.io/mapcube-example/index.html](https://overu.github.io/mapcube-example/index.html)

## Shanghai Palmap Intelligent Technology Co., Ltd (2013.09 ~ 2017.08)
### JavaScript 3D Map Rendering Engine
- JavaScript map rendering SDK, consistent with the 3D map engine (API, rendering effect), is also the main product, supporting indoor multi-floor interactive rendering on the same screen
- Based on three.js and also exploring WebGL, the more burdensome computational tasks (such as positioning algorithms) are placed in Web Worker
- Principal and lead programmer, from technology selection to core code writing, etc.

### Android 3D map rendering engine
- 3D map rendering SDK, the bottom layer uses C/C++ to implement a set of codes, which can run across Android, iOS, macOS, Windows, etc, supports custom map style through Lua
- Based on Irrlicht, shield the differences of graphics API of different platforms , not only can cross-platform, but also support cross-engine
- Principal and lead programmer, from technology selection to core code writing, compilation on Android side
- Did a lot of work on memory leaks, such as wrapping C++ objects, increasing reference counts, providing count stabilization when escaping to the Java layer, rendering optimizations, merging static POIs, and reducing rendering batches

### Android 2D map rendering engine
- 2D map rendering SDK, parsing and rendering of GeoJSON data, providing rich  interfaces for interaction
- Independent development, from 0 to 1, contact with Android 2D graphics API, have a preliminary understanding of graphics rendering, and have the concept of basic graphics  
- A lot of optimization practices. For example, map rendering with a POI of a certain magnitude will have stuck behavior, and map data needs to be segmented. Each segment is rendered by a thread, and then synthesized by the main thread

## Shanghai Retech Information Technology Co., Ltd. (2012.02 ~ 2013.08)
### Keruixing Preschool Education Platform
- A multimedia education platform for young children, supporting the distribution of multimedia courseware resources, providing real-time teaching, online multi-person collaboration, similar to Google Drive
- Referring to the technical characteristics of Google Wave, online multi-person collaboration is realized through real-time editing and conflict resolution strategies
- Responsible for front-end development, understand the concept of components and modules through the use of Google Closure, and contact Vert.x while helping to do part of the back-end development

### Readers
- An online reader based on HTLM5/CSS3
- Early exploration of Hybrid, compiling to different platforms by using PhoneGap (Apache Cordova), and implement Java to JavaScript conversion based on GWT
- Responsible for front-end development

---

## Amateur Program
### wx-compiler
Convert WeChat applet components (script, json, wxml, wxss) to Vue Component Render, supporting most of the syntax
- A lot of exploration and application to swc, esbuild
- wxml repl: [https://overu.github.io/wx-ast-explorer/index.html](https://overu.github.io/wx-ast-explorer/index.html)

### Unit Conversions
Used for unit conversion, Android App, it’s my own amateur practice, mainly to learn and understand RoboGuice (Google Guice extension, lightweight IoC framework).
- Link: [https://github.com/Overu/conversion](https://github.com/Overu/conversion)

---

## Skills
- Languages: JavaScript/TypeScript/Java/Kotlin/C/C++
- Front-end framework: Vue/React/ReactNative
- Front-end tools: vite/webpack/rollup
- Platform: Android/Electron/WeChat applet/Hybrid
- Other: WebGL/Node.js

## Thanks
Thank you for reading my resume carefully, due to the limited writing and unsatisfactory summary ability, there may be mistakes in many aspects, please bear with me. I would appreciate it if you could give me an interview opportunity

# JS Debug
## C 端调试
### chrome 调试
1. demo
2. 特性
### chrome inspect 调试 -- 安卓
1. 需要开发版的 `APP`
2. 翻墙
### safari 调试 -- ios
1. `safari` 打开的网页（XCode 打开的 webview）
2. 手机 `safari` 开启 `高级 -> 启用 “开发” ` 选项
3. mac `safari` 开启功能 `高级 -> Web 检查器`
## 调试脚本
### 代码调试
#### node debug
1. `node debug add.js`
2. `r(run)、continue(c)、next(n)、step(s)、out(p)`
#### node inspect
1. `node --inspect-brk add.js`
2. 浏览器打开 `chrome-devtools://devtools/bundled/js_app.html?experiments=true&v8only=true&ws=127.0.0.1:9229/dc9010dd-f8b8-4ac5-a510-c1a114ec7d29`
3. 访问 `chrome://flags/#enable-devtools-experiments` 开始 `devtools` 功能
#### vscode 调试
1. 配置 `launch.json`
### cli 代码调试
## Node 调试
## nodeServer 调试
1. `node --inpsect listen.js`
2. `chrome` 打开 `chrome::inspect`  `devtools` 上点击 `node` 图标
3. `vscode` 配置 `JSON`
### 调试 TS 
1. 编译 ts，带有 `souceMap`
2. 配置 `launch` 到对应的js文件

**任何带有 `sourceMap` 的文件都可以调试**
### 子进程调试
### 远程调试
## node 源码调试
### 代码配置步骤
1. 下载 `node` 源码、`CLion` 客户端
2. `sh configure` 执行配置文件 (1hous)
3. `make` 根据 `makefile` 的配置，进行编译，生成可执行文件
4. `make install` 安装 (半个小时)
### IDE 配置
1. 导入项目(`New Project`)，会生成对应的 `CMakeList.txt`（），以下是配置 `Debug` 参数
2. target -> node
3. executable -> out/Debug/node
4. program arguments -> test.js 新建调试脚本
5. working directory -> projectPath  工作目录脚本
6. Before launch 删除 build ，如果需要改代码 debug ，手动 make




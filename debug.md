% Debug

# 调试脚本
## node debug
1. `node debug add.js`
2. `r(run)、continue(c)、next(n)、step(s)、out(p)`

## node inspect
1. `node --inspect-brk add.js`
2. `chrome` 打开 `chrome::inspect`  `devtools` 上点击 `node` 图标
3. 打开 `devtools`, 点击 `Node` 图标


## vscode 调试
1. 配置 `launch.json`

# 升级版

## server 调试
1. `node --inpsect listen.js`
2. `vscode` 配置 `JSON`

## 调试 TS 
1. 编译 ts，带有 `souceMap`
2. 配置 `launch` 启动文件成编译后的js文件


## cli 调试

## 远程调试
1. `webstorm` 配置

# node 源码调试

## 代码配置步骤
1. 下载 `node` 源码 和 `CLion` 客户端
2. `sh configure` 执行配置文件 (1hours)
3. `make -C out BUILDTYPE=Debug -j 4` 根据 `makefile` 的配置，进行编译，生成可执行文件
4. `make install` 安装 (0.5hours)

## IDE 配置
1. 导入项目(`New Project`)
3. executable ⇒ out/Debug/node
4. program arguments ⇒ test.js 新建调试脚本
5. working directory ⇒ projectPath  工作目录脚本
6. Before launch 删除 build

# 真机调试

## 安卓
- 需要开发版的 `APP` 或者 `chrome`
- 打开 `chrome://inspect/#devices`

## IOS 
- `safari` 打开的网页（XCode 打开的 webview）
- 手机 `safari` 开启 `高级 ⇒ 启用 “开发” ` 选项
- Mac `safari` 开启功能 `高级 ⇒ Web 检查器`





# 订阅节点前端转换工具 (Subconverter Frontend)

这是一个纯前端实现的订阅与节点转换工具，旨在提供一个安全、本地化、无需依赖外部服务器的解决方案。它将两个核心功能整合在一个简洁网页页面中。

[Demo Pages](https://sp.hotrue.cc)

## ✨ 功能特性

本项目集成了两种主要的转换功能，通过标签页轻松切换：

### 1. 订阅链接转换

- **功能**： 将单个/多个节点链接、订阅地址或本地文件路径转换为Clash或通用Base64格式的订阅链接。
- **运行前提**： 需要在本地运行 [subconverter](https://github.com/asdlokj1qpi233/subconverter/releases "null") 软件，并使其监听在默认的 `http://localhost:25500` 地址。
- **优势**： 完全在本地生成转换链接，避免了使用在线转换服务时可能存在的节点信息泄露风险。

### 2. Socks节点生成

- **功能**： 读取一个Clash兼容的YAML配置文件，或者单个、多个节点以及订阅直链，并为其中的每一个代理（proxy）生成一个独立的本地Socks/HTTP混合端口监听。
- **自定义**： 用户可以自由指定监听的起始端口。
- **产出**： 自动生成新的Clash配置文件，并提供一键下载功能，方便在相关代理软件中直接使用。

## 🚀 为什么使用这个工具？

跨境电商业务过程需要在本地电脑配置多节点对应多端口的使用场景，而默认的本地代理节点客户端（如 Clash、V2RayN等工具）并没有相关功能设置。

- **指纹浏览器需要**：不同代理节点对应不同 Socks 端口，完美支持指纹浏览器（如：AdsPower Browser）

某些在线订阅转换服务虽然方便，但也存在一些不容忽视的问题：

- **安全风险**： 不可靠的在线服务可能记录并盗取您的节点信息。
- **功能限制**： 很多在线平台对转换的节点数量有限制。
- **稳定性**： 依赖于第三方平台的可用性，随时可能失效。

本工具通过纯前端技术完美地解决了这些问题：

- **绝对安全**： 所有操作均在您的浏览器中完成，代码完全开源，无任何数据上传，杜绝了信息泄露的可能。
- **无限制**： 转换节点的数量仅受限于您的设备性能。
- **本地运行**： “订阅链接转换”功能依赖于您自己在本地运行的`subconverter`实例，稳定可靠。

## 🛠️ 如何使用

1. 下载本项目中的 `index.html` 文件。
2. 用现代浏览器（如 Chrome, Edge, Firefox）打开这个 `index.html` 文件。
3. 根据您的需求，在两个标签页之间切换使用相应的功能。

**请注意**: “订阅链接转换”功能需要您预先在本地启动 `subconverter` 程序。

## 📦 依赖工具

为了完整使用本页面的所有功能，您可能需要以下工具：

- **本地订阅转换软件**： [subconverter](https://github.com/asdlokj1qpi233/subconverter/releases "null")
- **代理客户端 (示例)**： [v2rayN](https://github.com/2dust/v2rayN/releases "null")
- **视频教程参考**： [YouTube](https://www.youtube.com/watch?v=ZXanc7wpP9g&t=72s "null")

## ❤️ 鸣谢

- [tindy2013](https://github.com/tindy2013 "null") (subconverter及前端转换脚本原作者)
- [asdlokj1qpi233](https://github.com/asdlokj1qpi233 "null") (subconverter的维护者之一)
# 最重要的写在最前面

1. 易有云 2.0 还远未完善，目前是体验版，体验版！对于要求比较高的请等待正式版
2. 目前使用难度还比较大，请等待更多的使用教程再来使用
3. 目前我们会频繁更新，可能随时无法用！我们不会主动通知，应用内部也暂不支持消息通知
4. 易有云 2.0 跟易有云 1.0 一点关系都没有，请不要用 1.0 的账号登录 2.0，请看下面的帮助文档操作

# Linkease

易有云 2.0 相关文档与信息

未来易有云跟 ddnsto 是完全独立的两个产品，他们的官网也是独立的，维护的人员也是独立的。

未来官网地址： https://www.linkease.com （目前还没启用）

## 易有云 2.0 介绍

### 使命

致力于家庭存储的一站式解决方案。

易有云提供一套私有云为主，公有云为辅助的云存储解决方案，在保证易用性为前提，尽可能解决家庭存储的各种问题。

### 解决痛点

1. 公有云存储网络各种被限速，限制，数据不在自己身边
2. 私有云存储外网访问设置很麻烦
3. 不同平台的客户端需要单独寻找，平台之间协议无法兼容，体验无法一致
4. 数据备份是个大问题，设置太专业，还容易设置错误造成数据丢失

### 产品基础概念

1. 存储端

存储端是主要负责存储数据的设备，像路由器，NAS，Linux 服务器等可以作为存储端，一般存储端都接着大的硬盘。

存储端的最核心功能是，可以分享给多个用户使用

2. 用户终端

像手机、电脑，电视属于用户终端。用户终端负责管理存储端端数据，自己本身的存储能力有限。用户终端同一时刻只能登录一个用户。

3. 用户账号

一个登录的账号，一个用户可以在多个终端登录。

### 核心功能实现

1. 手机相册同步（最好手机拍完照自动同步到存储端）
2. 双向同步（文件被编辑自动触发保存到存储端）
3. 历史备份，生成快照（为用户保存最近半年的所有数据的历史版本）
4. 支持单终端同时管理多个存储端
5. 存储端支持多用户
6. 通信链路安全，保证通信链路加密，不同的用户使用不同的密钥
7. 通信链路智能选择（自动使用局域网链路，点对点链路，或者 CDN 节点链路）
8. 共有协议支持（目前核心要支持 SFTP、Samba、Webdav）
9. 全平台支持：iOS/Android/Windows/macOS/Android-TV

## 易有云下载

### 存储端下载

1. 威联通（[下载](https://firmware.koolshare.cn/binary/LInkEase/QNAP/)）
2. 群晖
3. Koolshare Merlin 
4. Koolshare 软路由
5. 宝塔面板
6. Docker
7. ReadyNAS
8. 树莓派
9. Linux 通用版本（[下载](https://firmware.koolshare.cn/binary/LInkEase/LinuxStorage)）
10. Window 存储端
11. MacOS 存储端

### 终端下载

1. Windows（[下载](https://firmware.koolshare.cn/binary/LInkEase/Client/LinkEaseWin.zip)）
2. macOS（[下载](https://firmware.koolshare.cn/binary/LInkEase/Client/LinkEase.dmg)）
3. iOS（[2.1全新开发中，暂时使用家家云](https://testflight.apple.com/join/YfsgRTZV)）
4. Android（[2.1开发中，临时版本下载](https://firmware.koolshare.cn/binary/LInkEase/Client/linkease.apk)）
5. Android-TV（未开发）
6. Linux 命令行版本（等待发布）

### 更新日志

#### 存储端

##### 0.2.68

修复序列号的错误，导致无法绑定设备

## 易有云 2.0 所有特性

下面这张表格，易有云未来完整版本的功能表，以及每个功能实现的版本号

### 存储端功能列表

TODO

| 功能 | 强CPU | 弱CPU |
|-|-|-|
|content1|content2|content3|

### 终端功能列表

TODO

| 功能 |iOS|Android|Windows|macOS|Android-TV|
|-|-|-|-|-|-|
|content1|content2|content3|-|-|-|

## 帮助文档

我们产品人员还没有写好使用手册，同时我们产品也还没有开发好安装向导，我暂时写一个简单的教程：

1. 先用 iOS 或者 Andriod 注册一个账号（目前仅支持手机号，微信不支持，电脑端也不支持注册账号）
2. 然后用 QNAP 或者 Linux 通用版安装一个存储端（必须有个存储端）
3. 访问存储端设备的 http://ip:8897/preweb/ 可以看到二维码或者序列号，以及存储的路径（本来这里应该有个安装向导，目前暂时没实现，存储路径也暂时不能修改）
4. 用手机扫码，或者用 Windows macOS 端添加设备，输入序列号
5. 终端与存储端绑定成功，存储端的第一个用户为设备管理员，进一步可以分享设备给其他用户
6. 目前电脑端功能相对好一些，手机端的 UI 跟交互将全部改版，请期待

TODO manual 文档实现

### 易有云 2.0 槽点

1. 终端之间暂时无法双向同步（解释：内核是支持的，但是 UI 交互还没开放）
2. 存储端路径暂时无法修改（解释：UI 还没有开放）
3. Windows 暂时没有存储端，优先级比较低！所以很多人无法快速体验新版本

## 收费价格

因为相比公有云，用户自己承担了硬盘与硬件的存储，所以易有云收费相对便宜。

易有云未来偏向基于时长与带宽收费，而自研的功能免费。（非自研的功能未来可能有，屏幕投屏，远程桌面，图片或视频编辑等给予第三方收费平台的研发，需要二次收费）

目前的版本不评估带宽，因为现在无法评估，我将尽最大努力给用户提供足够用户体验的服务器带宽。

易有云只对存储端收费，终端不收费。

| 套餐 |存储端数量|账号数量|在线终端数量|定价|
|-|-|-|-|-|
|周套餐|1|2|4| 1人民币/7天 |
|体验套餐|1|2|4| 18人民币/年 |
|基础套餐|1|3|8| 39人民币/年 |
|双享套餐|2|6|16| 59人民币/年 |

## 赞助

易有云是一个商业产品，应该合理收费来维持背后的团队的研发与运营。但是因为功能特性太多，导致研发一直无法开发收费与订单模块。如果用户对我们这个项目有足够信心，请赞助我们！




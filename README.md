Tickets

A local-first Android ticket and digital-pass manager built with Kotlin + Jetpack Compose.

Current Version

v7.0.0

versionCode = 700
versionName = "7.0.0"

v7.0.0 Highlights

智能地铁正式版

智能地铁正式版发布，支持包含港台在内的共40个中国城市和7个美国城市。

智能地铁围绕完整的实时行程体验设计，包括：

GPS 实时行程跟踪

当前站、上一站、下一站识别

区间进度计算

“我已到达下一站”手动推进

路线、站点、换乘信息

多城市线路颜色与线路数据

App、后台状态与实时通知统一同步

实时通知

当前支持三路实时通知能力：

Android Live Update

Samsung Now Bar / 实时窗口

Xiaomi SuperIsland

应用当前版本已移除 Honor 灵动胶囊与 OPPO 流体云相关实现，因此它们不属于 v7.0.0 的支持列表。

台湾地铁

台湾地区以 台北 作为统一接入城市，统一覆盖北北桃相关轨道线路：

TRTC：台北捷运

TYMC：桃园机场捷运

NTMC：新北环状线

其中桃园、新北不单独建立城市入口，统一归入台北。

澳门暂不属于当前 v7.0.0 的正式城市支持范围，后续接入。高雄捷运也暂不属于当前版本的台湾接入范围，后续再扩展。

主要功能

票据管理

车票 / 火车票

飞机票

演出票

门票

电影票

取餐码

取件码

配送码

本地票据分类、搜索、归档与排序

票据详情页

智能识别

ML Kit OCR

中文、英文、数字混合识别

QR Code / Barcode 识别

从图片提取票据信息

跨设备分享

NFC 一碰分享

QR Code 分享

Nearby

Wi-Fi Direct

Bluetooth

发送与接收动画

票据备份

JSON 备份

PDF 备份

本地恢复

票据活化

支持对完成使用的票据进行状态标记，并根据票据类型展示相应完成印章：

Ticket Type

Stamp

Train / Plane

ARRIVED

Movie

WATCHED

Event

ATTENDED

Admission

VISITED

Pickup

PICKED UP

Delivery

COLLECTED

技术栈

Kotlin

Jetpack Compose

MVVM + Clean Architecture

Room

Google ML Kit

CameraX

ZXing

Google Nearby

Firebase Cloud Messaging

Cloudflare Workers + R2（城市轨道交通数据服务）

数据与隐私

Tickets 以本地数据管理为核心。票据数据默认保存在设备本地。

智能地铁的城市、线路、车站等公共交通数据通过对应的数据服务获取，并在应用侧进行缓存，以改善离线和网络异常时的可用性。

支持平台

中国

智能地铁正式版支持包含港台在内的 40 个中国城市。

美国

支持 7 个美国城市。

Release History

v7.0.0

智能地铁正式版发布，支持包含港台在内的共40个中国城市和7个美国城市

GPS 实时行程跟踪

当前站 / 上一站 / 下一站状态识别

区间进度与剩余行程计算

“我已到达下一站”手动推进

三路实时通知统一同步

多城市线路、站点、换乘支持

线路颜色数据支持

台湾北北桃统一接入台北城市入口

稳定性与后台运行体验优化

v6.0.0

NFC 一碰分享票据

QR Code 分享票据

JSON / PDF 备份票据

票据活化与呼吸光效

完成使用盖章

票据详情视觉更新

系统集成整理

v5.0.0

QR Code / Barcode

智能票据识别

Wallet 风格票夹视图

票据详情页

实时通知能力

系统体验优化

v4.0.0

搜索与智能排序

票据归档

分享与复制

JSON 备份

QR Code / Barcode

普通票据提醒

通知与实时活动

UI / 系统集成优化

输入、识别与性能优化

v3.0.0

实时活动

取餐码 / 取件码

票据使用体验优化

识别与设置优化

性能优化

v2.0.0

多票据类型

智能识别

系统集成

设置页面

v1.0.0

正式版本发布

本地票据管理

提醒与实时活动

智能能力

基础界面

License

This project is provided for personal use and development.

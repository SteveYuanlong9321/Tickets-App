票据 Tickets

票据 Tickets 是一个以本地票据管理为核心的 Android App，使用 Kotlin + Jetpack Compose 构建。项目同时集成票据识别、二维码/条形码、系统实时通知和智能地铁等能力。

当前版本

v7.0.0

versionCode: 700

versionName: 7.0.0

compileSdk: 37

targetSdk: 37

minSdk: 26

v7.0.0

智能地铁正式版

智能地铁从测试功能进入正式版本，支持站点搜索、路线规划、换乘信息和实时行程状态跟踪。

GPS 实时行程跟踪

根据设备定位持续判断当前站、上一站、下一站以及区间进度，并在应用切换到后台后继续保持行程状态。

四路实时通知同步

智能地铁状态统一同步到：

App 内智能地铁卡片

Android Live Update

Samsung Now Bar / 实时窗

小米超级岛

普通 Ongoing 回退通知

各通道共享当前站、下一站、换乘和进度状态。

手动到站

实时通知加入“我已到达下一站”。点击后立即推进当前行程，并同步更新 App 与实时通知状态；退出 App 后不会因为旧定位状态把行程拉回上一站。

多城市地铁

当前版本支持中国大陆多个城市、香港，以及已接入的美国主要城市。

当前美国地铁数据覆盖 7 个城市：

New York City

Washington, DC

Boston

Philadelphia

Chicago

San Francisco Bay Area

Los Angeles

台湾智能地铁：台北（北北桃统一）

7.0.0 的最新开发阶段已经加入台湾 TDX 数据接入架构。

App 中只建立一个台湾城市：

cityId = taipei

显示名称：

台北

统一包含：

台北捷运 TRTC

桃园机场捷运 A 线 TYMC

新北环状线 Y 线 NTMC

桃园、新北不作为独立城市。

台湾 Android 数据链路：

Android → Cloudflare Worker → TDX → 统一静态索引 → R2 → Android

公开读取接口：

GET /api/v1/tw/taipei/index

当前台湾静态数据使用 7 天本地缓存；网络不可用时可继续使用已有缓存。

注意：台湾 R2 与纽约 R2 正准备进一步隔离。最终部署建议为台湾独立 R2 binding，避免影响现有 NYC 数据。

路线与线路颜色

根据城市、线路和换乘状态自动选择对应线路颜色，并保持当前站、下一站、换乘线路和路线顺序一致。

稳定性

完善后台/前台切换、手动到站后的状态恢复，以及旧路线初始化和旧定位回调覆盖问题的处理。

票据功能

电影票、车票、机票、演出、门票

取餐码、取件码

二维码与条形码录入

相机扫码识别

本地 OCR

在线识别配置

票据搜索与智能排序

收藏与归档

JSON 备份与恢复

PDF 导出

NFC 一碰分享

二维码分享

系统实时集成

项目包含以下实时通知通道：

Android Live Update

Samsung Now Bar / 实时窗

小米超级岛

普通 Ongoing 通知回退

智能地铁实时状态使用统一数据模型，避免不同厂商通道出现当前站、线路颜色和换乘信息不一致。

数据与隐私

票据数据默认保存在当前设备。

美国部分地铁数据通过项目的 Cloudflare Worker / 本地静态数据链路提供。

台湾部分采用 TDX 数据源，并通过 Worker 生成统一索引。Android 不直接保存 TDX Client Secret。

构建

使用 Android Studio 打开项目后：

Sync Project with Gradle Files

确认 app 模块使用 versionCode = 700 和 versionName = "7.0.0"

Build > Make Project

测试完成后生成 Release APK

7.0.0 关键文件

MainActivity_7.0.0_SmartSubway_Release.kt

GlobalSubwayData_7.0.0_Taiwan_TDX_NorthNorthTaoyuan.kt

Worker_Taiwan_TDX_NorthNorthTaoyuan_8.2.js

update_7.0.0.json

GitHub Release

建议 Release 标签：

v7.0.0

建议 Release 标题：

Tickets v7.0.0 — Smart Subway

APK：

app-release.apk

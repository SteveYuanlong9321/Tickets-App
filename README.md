# Tickets-App
Tickets·票据

一款基于 Android / Kotlin / Jetpack Compose 的数字票据管理 App。

当前版本
6.0.0

主要功能
电影票、车票、机票、演出、门票、取餐码、取件码统一管理
二维码 / 条形码录入、相机识别与详情展示
NFC 一碰分享票据
二维码分享票据
Android 系统分享
JSON / PDF 票据备份与恢复
Live Update 实时票据通知
Samsung Now Bar
小米超级岛
桌面 Widget
票据搜索、收藏、自动归档
票据使用状态与“使用完成”盖章
票据活化视觉效果

6.0.0 新增内容
票据活化
票据在接近行程开始或进行中时显示柔和的无边界呼吸光效。
光效采用整体色彩呼吸，不使用扫描线、进度线、位移流动或明显阴影轮廓，并使用对应票据类型的主题色。
票夹页卡片与票据详情页保持统一视觉效果。
使用完成盖章
手动将票据标记为已使用后，呼吸光效停止，同时显示印章：
机票：ARRIVED
车票：ARRIVED
电影票：WATCHED
演出：ATTENDED
门票：VISITED
取餐码：PICKED UP
取件码：COLLECTED
票夹页印章位于简略卡片右侧；详情页印章位于二维码 / 条形码区域。

6.0.0 其他更新
NFC 一碰分享票据
二维码分享票据
JSON / PDF 备份与恢复
系统集成整理
桌面 Widget 全尺寸适配
二维码 / 条形码详情展示
Live Update、Samsung Now Bar 与小米超级岛相关体验整理

构建环境
Android
Kotlin
Jetpack Compose
Material 3
compileSdk 37
minSdk 26
targetSdk 37

说明
本项目主要用于个人票据整理、设备集成和视觉体验实验。

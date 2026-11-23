# JQ Viewer（优化线路版）

JMComic 第三方漫画阅读器，支持 Android 移动端和 Windows、Linux 桌面端。它把搜索、收藏、下载、本地阅读、PDF 导入导出和批量解析放在同一套界面里，方便整理和阅读漫画。

> 本仓库是 [JQ Viewer](https://github.com/JUKOMU/JQ-Viewer) 的**优化线路版本**：源码沿用上游原版，版权归原作者 JUKOMU 所有，遵循 MIT License，这里只发布优化线路后的安装包和版本说明。

[![Version](https://img.shields.io/badge/Version-2.2.3%20mod%20v6-brightgreen.svg)](https://github.com/hdjcj496749/JQ-Viewer/releases)
[![Android](https://img.shields.io/badge/Android-7.0%2B-3DDC84?logo=android&logoColor=white)](https://github.com/hdjcj496749/JQ-Viewer/releases)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> JQ Viewer 是个人项目，与 JMComic 官方无关。项目本身不包含漫画资源，请遵守所在地法律法规和目标站点规则。

## 下载

| 版本 | 安装包 | SHA-256 |
| --- | --- | --- |
| 2.2.3 mod v6 | [JQViewer_2.2.3_mod_v6.apk](https://aka.doubaocdn.com/s/IMY5j0dVuS) | `d421425169edd61b150ad211595473beb0f3f99a165c460b7a2449c8d89214b7` |

- Android 7.0 及以上。
- 安装包签名与原版不同，若手机上已装原版，请先卸载再安装；卸载会清除应用内的收藏和设置，建议提前备份。
- 版本说明见 [docs/releases/v2.2.3-mod-v6.md](docs/releases/v2.2.3-mod-v6.md)。

## 本版改动

- 新增可用线路，API 线路固定为当前可用的 8 条。
- 图片线路探测改为多路并发：4 路分批，每条线路 5 张图 × 2 轮，缩短首图等待时间。
- 其他功能与上游 2.2.3 保持一致。

线路可达性会随网络和地区变化，加载失败时可在设置中切换线路。

## 使用文档

使用说明见 [用户文档](docs/sources/index.md)，涵盖安装、搜索、阅读、收藏、下载导出、历史、设置和常见问题。

## 项目说明

本仓库是上游 [JUKOMU/JQ-Viewer](https://github.com/JUKOMU/JQ-Viewer) 的 fork，源码保持上游原样，不在此仓库维护代码改动。桌面端（Windows/Linux）请前往 [上游 Releases](https://github.com/JUKOMU/JQ-Viewer/releases) 下载。

| 平台 | 支持情况 |
| --- | --- |
| Android | 支持 Android 7.0 及以上版本（本仓库提供优化线路版 APK） |
| Windows | 支持 Windows x64；Windows on ARM 使用 x64 应用仿真（上游发行包） |
| Linux | 支持 x64 和 arm64（上游发行包） |

---

## 应用截图

<details open><summary></summary>
  
### 首页、搜索、分类

| 首页 | 搜索 | 分类 |
| --- | --- | --- |
| <img width="260" alt="首页" src="https://github.com/user-attachments/assets/b3979725-d2e7-4721-92c1-5181aa160ca9" /> | <img width="260" alt="搜索" src="https://github.com/user-attachments/assets/158b13ed-396d-4add-be2e-d7d415648c44" /> | <img width="260" alt="分类" src="https://github.com/user-attachments/assets/b12c77fe-1231-4485-bad5-5b45a275d308" /> |

### 详情与阅读

| 详情页 | 章节选择 | 预览 |
| --- | --- | --- |
| <img width="260" alt="详情页" src="https://github.com/user-attachments/assets/a66e92ed-4819-446c-a8d5-e72021345af8" /> | <img width="260" alt="章节选择" src="https://github.com/user-attachments/assets/12dffcf1-d205-4ee0-9897-e14c1d37466d" /> | <img width="260" alt="预览" src="https://github.com/user-attachments/assets/fe24724b-59a7-4f24-b3fa-151a806e5275" /> |

| 评论 | 阅读器 | 阅读设置 |
| --- | --- | --- |
| <img width="260" alt="评论" src="https://github.com/user-attachments/assets/e4cf5d50-c811-4aa6-b57a-67ad6ed00a5f" /> | <img width="260" alt="图片阅读器" src="https://github.com/user-attachments/assets/125e157f-d505-44ba-ac87-e2e6fcbd2f95" /> | <img width="260" alt="阅读设置" src="https://github.com/user-attachments/assets/17648ad7-85b0-435c-877c-e8639d6733a4" /> |

### 收藏与历史

| 收藏夹 | 收藏夹搜索 | 浏览历史 |
| --- | --- | --- |
| <img width="260" alt="收藏夹" src="https://github.com/user-attachments/assets/9890ecad-ad3b-48a7-a2f1-f6497cd3ec5b" /> | <img width="260" alt="收藏夹搜索" src="https://github.com/user-attachments/assets/c669cf81-e5a2-43e5-91ad-fd468fdb9b75" /> | <img width="260" alt="浏览历史" src="https://github.com/user-attachments/assets/986400a7-3081-4f04-bc9e-afc80e7ae1f2" /> |

| 解析历史 | 批量解析 |
| --- | --- |
| <img width="260" alt="解析历史" src="https://github.com/user-attachments/assets/da2b69b0-1d09-489c-8f54-c31757926f8a" /> | <img width="260" alt="批量解析" src="https://github.com/user-attachments/assets/614b2ea7-94e3-4c42-b84f-a74a9296e5a7" /> |

### 下载与 PDF

| 下载队列 | 下载管理 | 后台进度 |
| --- | --- |---|
| <img width="260" alt="下载队列" src="https://github.com/user-attachments/assets/85aef0b1-d80e-44c9-a02a-29379a9806c8" /> | <img width="260" alt="下载管理" src="https://github.com/user-attachments/assets/6f227a1c-efa5-4788-ae1f-b96c83e0cbae" /> | <img width="260" alt="下载通知" src="https://github.com/user-attachments/assets/083a4bb5-c8a7-43e2-b1ea-80dc7bb6b4b8" /> |

| PDF 导出 | 多章节导出 | PDF 导入匹配 |
| --- | --- |---|
| <img width="260" alt="PDF 导出" src="https://github.com/user-attachments/assets/b61c714b-4a2a-4ac5-a215-6a03a3bdaea8" /> | <img width="260" alt="多章节导出" src="https://github.com/user-attachments/assets/731de6a5-be0b-424e-b6cc-a4fc6f8fe044" /> | <img width="260" alt="PDF 导入匹配" src="https://github.com/user-attachments/assets/475ad932-c96c-4a24-bf4b-5d64faa6e5f3" /> |

| PDF 管理 |  |  |
| --- | --- | --- |
| <img width="270" alt="PDF 管理" src="https://github.com/user-attachments/assets/6a54aa72-4d64-46ed-b48d-b4d5e716b328" /> | <img width="270" alt="PDF 管理" src="https://github.com/user-attachments/assets/4e4f9154-c5f6-4d24-939d-dbf22937ef50" /> | <img width="270" alt="PDF 管理" src="https://github.com/user-attachments/assets/76429244-172f-43fa-8946-6f1b3543ec22" /> |

### 设置

| 查看图片缓存 | 查看网络状态 | 导出设置 |
| --- | --- |---|
| <img width="260" alt="查看图片缓存" src="https://github.com/user-attachments/assets/35fc1994-161c-46f8-8415-d89499905859" /> | <img width="260" alt="查看网络状态" src="https://github.com/user-attachments/assets/4229b9bb-203a-4e24-860e-c7a378337c26" /> | <img width="260" alt="下载通知" src="https://github.com/user-attachments/assets/50a0ea1f-0e0c-4ca0-a203-f5d17bb897b8" /> |

</details>
  
---

## 主要功能

### 内容检索

- 关键词、ID、作者、标签、登场人物等搜索方式。
- 分类浏览、排序筛选和时间范围筛选。
- 搜索历史按场景保存，便于重复检索。

### 阅读体验

- 支持横向翻页和纵向滚动两种阅读方式。
- 可调亮度、防息屏、音量键翻页、屏幕方向等阅读设置。
- 已下载图片和已导入 PDF 可以直接从详情页或下载页打开。

### 收藏与记录

- 支持在线收藏夹，也支持不登录时使用离线收藏夹。
- 收藏夹内搜索、移动、复制、批量下载和文本导出。
- 浏览历史、解析历史自动记录，方便回到之前看过或处理过的内容。

### 离线与导出

- 章节下载队列支持暂停、恢复、重试和删除。
- 下载完成后可离线阅读，也可以按需公开到系统相册。
- PDF 导出支持自定义目录、文件名模板、分卷和后台进度通知。
- 本地 PDF 可以导入应用，并尽量匹配到对应作品和章节。

### 批量解析

- 从多行文本里批量提取 ID，再统一搜索、收藏或下载。
- 可选 OCR 识别图片中的文字，用来辅助处理截图里的编号。

---

## 安装

本仓库只提供 Android 端的优化线路版 APK，前往本仓库 Releases 下载。桌面端请前往 [上游 Releases](https://github.com/JUKOMU/JQ-Viewer/releases)。

- Android：下载 APK 安装。应用内可以在“设置 > 关于 > 检查更新”查看最新版本。
- Windows：下载安装版 EXE，或使用便携版 ZIP（上游发行包）。
- Linux：下载 DEB、RPM 安装包，或使用便携版 TAR.GZ（上游发行包）。

---

## 开发构建

源码与上游一致，构建方式请参考 [上游仓库](https://github.com/JUKOMU/JQ-Viewer)。项目主体是 Vue 3 + Ionic。Android 端使用 Capacitor 和原生插件，负责下载、缓存、PDF、OCR 等能力；Desktop 端使用 Java 21 宿主和本地服务提供对应能力。接口调用依赖 [JMComic-Api-Java](https://github.com/JUKOMU/JMComic-Api-Java)。

通用构建环境需要 Node.js、JDK 21 和 Maven。构建 Android 还需要 Android SDK：

```bash
npm install
npm run build
```

构建 Android Debug APK：

```bash
npm run build:android
```

同步并构建 Desktop 前端和 Java 宿主：

```bash
npm run desktop:sync -- --platform windows
mvn -f desktop/pom.xml package
```

---

## 许可证

[MIT License](LICENSE)，版权归原作者 JUKOMU 所有。

# 🎮 英雄联盟 · 全英雄阵营 / 地区 + 皮肤图鉴

一个轻量、零依赖、可离线运行的**单文件交互式网页**，收录《英雄联盟》（端游）：

- **173 位英雄**，按官方《英雄联盟》宇宙的 **14 个地区** 分类，支持按**定位**筛选、按**发布时间**浏览
- **1943 款皮肤**，按 **225 个皮肤系列**（平行时空宇宙）归类，与英雄**双向跳转**
- 每位英雄含官方**中文简介**、职业定位、难度与**上线日期**
- 一张**可交互的符文之地地图**，点击地区标记即可漫游该地区英雄

> 🌐 **在线预览**：`https://loctyan.github.io/lol-champions-regions/`
>
> ⬇️ 本地使用：直接双击 `index.html` 用浏览器打开即可。

![heroes](https://img.shields.io/badge/英雄-173-0ac8b9) ![skins](https://img.shields.io/badge/皮肤-1943-c8aa6e) ![lines](https://img.shields.io/badge/皮肤系列-225-7d6bb8) ![regions](https://img.shields.io/badge/地区-14-4b8bdf) ![date](https://img.shields.io/badge/数据截至-2026.09.09-8b96ad)

---

## ✨ 功能特性

### 英雄图鉴
- 🔍 **实时搜索**：中文名 / 英文名 / 称号 / 阵营 / 定位
- 🏷️ **地区 + 定位筛选**：14 个地区 × 6 大定位（战士 / 坦克 / 法师 / 刺客 / 射手 / 辅助），可叠加过滤
- 📅 **三种浏览模式**：按地区分组 / 按名称排序 / **按发布时间**（自动按年份分组为时间轴）
- 📖 **英雄档案**：官方中文简介、职业定位、难度、上线日期
- 🖼️ **高清原画**：弹窗展示官方原画（1215×717，官方最高清版本），点击可**全屏放大**查看
- 🔗 **英雄 ⇄ 皮肤双向跳转 + 皮肤翻页**：英雄弹窗内列出其全部皮肤（点击进入详情）；皮肤弹窗顶部有 **`← 查看原皮`** 按钮和 **`‹ ›` 翻页器**（显示 `5 / 18` 位置，支持 **←/→ 方向键**），可在同一英雄的皮肤间直接切换，无需反复回到原皮

### 符文之地地图
- 🗺️ **官方交互地图**：直接嵌入 Riot 官方《符文之地地图》（`map.leagueoflegends.com`）——可缩放、拖动、点击地点查看故事，**零维护、随官方更新**
- 📍 **14 个地区卡片**：与本地数据联动，点击即展开该地区全部英雄，再点一次取消选中
- 🌌 **非地理地区说明**：虚空之地（异次元虚空）／班德尔城（隐秘约德尔城邦）／符文之地（无固定归属）单独标注

### 皮肤图鉴
- 🌌 **按皮肤系列分组**：225 个平行时空宇宙（源计划、灵魂莲华、K/DA、星之守护者…），可折叠展开
- 🦸 **按英雄分组**：一键切换，查看某位英雄的全部皮肤
- 🔍 **跨字段搜索**：皮肤名 / 英雄名 / 系列名
- 🖼️ **原画弹窗**：皮肤展示官方高清原画，同样支持点击全屏放大
- ⚡ **性能优化**：分组默认折叠、按需渲染 + 图片懒加载

---

## 📊 地区分布（14 地区 · 173 英雄 · 1943 皮肤）

| 地区 | 英雄 | 皮肤 | 地区 | 英雄 | 皮肤 |
| --- | --- | --- | --- | --- | --- |
| 德玛西亚 | 15 | 200 | 暗影岛 | 10 | 90 |
| 诺克萨斯 | 17 | 169 | 班德尔城 | 7 | 89 |
| 艾欧尼亚 | 23 | 283 | 巨神峰 | 7 | 87 |
| 皮尔特沃夫 | 8 | 107 | 以绪塔尔 | 8 | 78 |
| 祖安 | 14 | 159 | 虚空之地 | 9 | 86 |
| 弗雷尔卓德 | 15 | 155 | 符文之地 | 21 | 238 |
| 恕瑞玛 | 11 | 106 | 比尔吉沃特 | 8 | 96 |

## 🌌 主要皮肤系列（Top 12）

| 系列 | 数量 | 系列 | 数量 |
| --- | --- | --- | --- |
| 珍宝 | 82 | 泳池派对 | 26 |
| 西部风云 | 38 | 腥红之月 | 25 |
| 灵魂莲华 | 35 | 不给糖就捣蛋 | 22 |
| 职场精英 | 34 | 胜利诸神 | 22 |
| 源计划 | 33 | 魔女 | 22 |
| 黑夜使者和黎明使者 | 28 | 暗星 | 22 |

---

## 🚀 快速开始

### 本地运行
无需任何环境，直接用浏览器打开 `index.html` 即可；也可以用任意静态服务器：

```bash
python -m http.server 8000     # 或
npx serve .
```

### 部署到 GitHub Pages
1. 新建**公开**仓库，把 `index.html` 上传到仓库根目录
2. `Settings → Pages`，Source 选 `Deploy from a branch`，Branch 选 `main`，目录选 `/ (root)`
3. 保存后等待约 1 分钟，访问 `https://用户名.github.io/仓库名/`

> 也可以拖拽到 [Netlify Drop](https://app.netlify.com/drop) 或 [Cloudflare Pages](https://dash.cloudflare.com) 上传，同样免费。

---

## 🛠 技术说明

- **纯 HTML + CSS + 原生 JavaScript**，无框架、无构建、无第三方依赖，数据全部内联在单个文件中
- 弹窗使用 Riot Games 官方原画（[Data Dragon](https://developer.riotgames.com/docs/lol#data-dragon) `splash`，1215×717 —— 这也是 Riot 官网自己使用的最高清版本），支持点击全屏放大；卡片缩略图使用官方向导立绘（`loading`，308×560），离线时自动降级为纯色首字母头像
- 符文之地地图为 **iframe 嵌入 Riot 官方地图**（官方站点无 `X-Frame-Options` 与 CSP `frame-ancestors` 限制，可安全嵌入），不占本页体积，且随官方更新；若被网络或浏览器拦截，页面提供了「在新标签页打开」的直达链接
- 卡片配色按地区主题色区分，深色主题贴合英雄联盟视觉风格
- 皮肤列表默认折叠、展开时才渲染 DOM，配合 `loading="lazy"` 控制 1900+ 图片的加载

---

## 🔄 数据维护

页面内有两块数据，都在 `index.html` 中：

### 1. 英雄数据
```js
// [中文名, 英文名, 中文称号, 地区key, DataDragon头像id, 阵营(可空)]
["亚托克斯", "Aatrox", "暗裔剑魔", "runeterra", "Aatrox", "暗裔"],
```
- **地区 key**：`demacia / noxus / ionia / piltover / zaun / freljord / shurima / bilgewater / shadowisles / bandlecity / targon / ixtal / void / runeterra`
- **阵营**：`暗裔`、`光之哨兵`、`恶魔` 等跨地区标签

### 2. 皮肤数据
```js
const SKIN_LINES = ["珍宝", "西部风云", ...];      // 系列名（按皮肤数降序）
const SKINS = [ ["Aatrox", 1, "铁血剑豪 亚托克斯", 12], ... ];  // [英雄id, 编号, 皮肤名, 系列下标]
```
- 头像/原画 URL 由 `英雄id` + `编号` 拼出：`.../loading/{英雄id}_{编号}.jpg`
- 新增皮肤时追加一行；系列下标指向 `SKIN_LINES`，`-1` 表示无系列

### 3. 英雄扩展数据（职业 / 难度 / 上线日期 / 简介）
```js
const ROLES = ["Fighter","Tank","Mage","Assassin","Marksman","Support"];
const ROLE_CN = { Fighter:"战士", Tank:"坦克", ... };
// 与 DATA 一一对应：[职业下标, 难度(0-10), 上线日期, 中文简介]
const CMETA = [ [[0,1], 4, "2013-06-13", "……"], ... ];
```
- 与 `DATA` 数组**按下标一一对应**，新增英雄时两处同时追加即可

### 4. 符文之地地图
地图**不占用本页任何体积** —— 直接 iframe 嵌入 Riot 官方地图，改一个常量即可切换语言版本：

```js
const OFFICIAL_MAP = "https://map.leagueoflegends.com/zh_TW/";  // 亦可换 en_US / ja_JP / ko_KR …
```

---

## 📌 数据说明

- 数据截至 **2026 年 9 月 9 日**（最新英雄：灰烬驱魔人 · 洛克）
- 英雄地区划分以《英雄联盟》宇宙官网（yz.lol.qq.com）为准
- **「符文之地」** 为官方兜底分类，指无固定地区、四处游历或宇宙 / 恶魔类存在
- **「暗裔」** 为跨地区阵营，官方按现居地归入各地区（亚托克斯 → 符文之地、纳亚菲利 → 恕瑞玛、韦鲁斯 → 艾欧尼亚、亚恒 → 符文之地）
- 皮肤数据来自 Riot 客户端数据（CommunityDragon），**不含各英雄的默认皮肤与旧版「经典」皮肤**
- 皮肤系列即官方 skinLines 字段，因部分系列按赛季拆分（如「星之守护者 第四季」），故系列数偏多
- 英雄简介、职业定位、难度来自 Data Dragon；上线日期来自 [《英雄联盟》Wiki 数据模块](https://leagueoflegends.fandom.com/wiki/Module:ChampionData/data)（2025-2026 三位新英雄由手工补录）
- 符文之地地图由 [Riot Games 官方](https://map.leagueoflegends.com/) 提供并直接嵌入，本页不复刻、不缓存
- 诺拉（Norra）为《英雄联盟手游》专属英雄，未计入端游名单

---

## 📚 数据来源

- [《英雄联盟》宇宙官网 · 英雄列表](https://yz.lol.qq.com/zh_CN/champions/) — 地区划分与英雄名单
- [腾讯英雄联盟 · 游戏资料库](https://lol.qq.com/data/info-heros.shtml) — 中文称号
- [CommunityDragon](https://raw.communitydragon.org/latest/plugins/rcp-be-lol-game-data/global/zh_cn/v1/skins.json) — 皮肤、皮肤系列（官方客户端数据）
- [Data Dragon](https://developer.riotgames.com/docs/lol#data-dragon) — 官方原画（`splash`，1215×717）与立绘缩略图（`loading`）
- [League of Legends Wiki](https://leagueoflegends.fandom.com/wiki/List_of_champions)

---

## ⚖️ 版权声明

本项目仅供学习与交流使用。英雄联盟（League of Legends）及相关角色、皮肤、图像、名称版权均归**拳头游戏（Riot Games）** 所有，请勿用于商业用途。

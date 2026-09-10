# 🎮 英雄联盟 · 全英雄阵营 / 地区图鉴

一个轻量、零依赖、可离线运行的**单文件交互式网页**，收录《英雄联盟》（端游）全部 **173 位英雄**，并按照官方《英雄联盟》宇宙的 **14 个地区** 分类展示。

> 🌐 **在线预览**：`https://loctyan.github.io/lol-champions-regions/`
>
> ⬇️ 本地使用：直接双击 `index.html` 用浏览器打开即可。

![heroes](https://img.shields.io/badge/英雄-173-0ac8b9) ![regions](https://img.shields.io/badge/地区-14-c8aa6e) ![size](https://img.shields.io/badge/单文件-无依赖-7abd63) ![date](https://img.shields.io/badge/数据截至-2026.09.09-8b96ad)

---

## ✨ 功能特性

- 🔍 **实时搜索**：支持中文名 / 英文名 / 称号 / 阵营关键词（如「亚索」「Yasuo」「暗裔」「光之哨兵」）
- 🏷️ **地区筛选**：14 个地区标签一键过滤，实时显示各地区英雄数量
- 🗂️ **双浏览模式**：按地区分组 / 按名称（拼音）排序
- 🖼️ **详情弹窗**：点击卡片查看官方立绘大图 + 称号、地区、阵营
- 📊 **统计面板**：英雄总数、地区数、暗裔英雄一览
- 📱 **响应式布局**：适配手机 / 平板 / 桌面端

---

## 📊 地区分布（14 地区 · 173 英雄）

| 地区 | 数量 | 地区 | 数量 |
| --- | --- | --- | --- |
| 德玛西亚 Demacia | 15 | 暗影岛 Shadow Isles | 10 |
| 诺克萨斯 Noxus | 17 | 班德尔城 Bandle City | 7 |
| 艾欧尼亚 Ionia | 23 | 巨神峰 Targon | 7 |
| 皮尔特沃夫 Piltover | 8 | 以绪塔尔 Ixtal | 8 |
| 祖安 Zaun | 14 | 虚空之地 The Void | 9 |
| 弗雷尔卓德 Freljord | 15 | 符文之地 Runeterra | 21 |
| 恕瑞玛 Shurima | 11 | 比尔吉沃特 Bilgewater | 8 |

---

## 🚀 快速开始

### 本地运行
无需任何环境，直接用浏览器打开 `index.html` 即可；也可以用任意静态服务器：

```bash
# Python
python -m http.server 8000
# Node
npx serve .
```

然后访问 `http://localhost:8000`。

### 部署到 GitHub Pages

1. 新建**公开**仓库，把 `index.html` 上传到仓库根目录
2. 进入 `Settings → Pages`，Source 选 `Deploy from a branch`，Branch 选 `main`，目录选 `/ (root)`
3. 保存后等待约 1 分钟，即可通过 `https://用户名.github.io/仓库名/` 访问

> 也可以拖拽到 [Netlify Drop](https://app.netlify.com/drop) 或 [Cloudflare Pages](https://dash.cloudflare.com) 直接上传，同样免费。

---

## 🛠 技术说明

- **纯 HTML + CSS + 原生 JavaScript**，无框架、无构建、无第三方依赖
- 英雄立绘/头像来自 Riot Games 官方 CDN（[Data Dragon](https://developer.riotgames.com/docs/lol#data-dragon)），以 `<img>` 外链方式加载，离线时自动降级为纯色首字母头像
- 卡片颜色按地区主题色区分，深色主题贴合英雄联盟视觉风格

---

## 🔄 数据维护

所有数据集中存放在 `index.html` 顶部的 `const RAW = [...]` 数组中，每条格式：

```js
// [中文名, 英文名, 中文称号, 地区key, DataDragon头像id, 阵营(可空)]
["亚托克斯", "Aatrox", "暗裔剑魔", "runeterra", "Aatrox", "暗裔"],
```

- **地区 key**：`demacia / noxus / ionia / piltover / zaun / freljord / shurima / bilgewater / shadowisles / bandlecity / targon / ixtal / void / runeterra`
- **阵营**：`暗裔`、`光之哨兵`、`恶魔` 等跨地区标签，无则留空
- **新英雄上线**：追加一行即可，页面会自动更新总数与地区计数

---

## 📌 数据说明

- 数据截至 **2026 年 9 月 9 日**（最新英雄：灰烬驱魔人 · 洛克）
- 地区划分以《英雄联盟》宇宙官网（yz.lol.qq.com）为准
- **「符文之地」** 为官方兜底分类，指无固定地区、四处游历或宇宙/恶魔类存在（如瑞兹、千珏、巴德等）
- **「暗裔」** 为跨地区阵营，官方按现居地归入各地区（亚托克斯→符文之地、纳亚菲利→恕瑞玛、韦鲁斯→艾欧尼亚、亚恒→符文之地）
- 诺拉（Norra）为《英雄联盟手游》专属英雄，未计入端游名单

---

## 📚 数据来源

- [《英雄联盟》宇宙官网 · 英雄列表](https://yz.lol.qq.com/zh_CN/champions/)
- [腾讯英雄联盟 · 游戏资料库](https://lol.qq.com/data/info-heros.shtml)
- [League of Legends Wiki · List of champions](https://leagueoflegends.fandom.com/wiki/List_of_champions)
- [Universe of League of Legends · Regions](https://universe.leagueoflegends.com/en_US/regions/)

---

## ⚖️ 版权声明

本项目仅供学习与交流使用。英雄联盟（League of Legends）及相关角色、图像、名称版权均归**拳头游戏（Riot Games）** 所有，请勿用于商业用途。

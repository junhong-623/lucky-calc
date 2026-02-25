# 🏮 幸运计算 · Lucky Calculator Palace

> 专为马来西亚华人打造的多功能计算工具 —— 4D 彩票、牛牛、赔率、利息，一站搞定。

**🌐 Live Site → [junhong-623.github.io/lucky-calc](https://junhong-623.github.io/lucky-calc)**

---

## ✨ 功能一览

### 🎰 普通计算器
- 基础四则运算（+ − × ÷）
- 支持键盘输入（数字键、Enter、Backspace、Esc）
- 连续按 `=` 可重复上一次运算（如 `1+1=2` → 再按 `=` → `3` → `4`）

### 🀄 幸运 4D
- 随机生成幸运号码 + 专属祝福语
- 一键生成 5 个号码备选
- **千字图查询**：自动查出号码对应的中文 / 英文名称（万字书）
- 快速跳转 check4d.org 查询历史中奖记录

### 🃏 牛牛计算器
- 五张牌点击选牌，自动算出最佳拆法
- 支持 **3↔6 灵活模式**：开启后系统自动尝试所有 3/6 组合，取最高得分
- 特殊牌型：**♠A 天王牌**（黑桃A + JQK，底三张需整数）
- 结果清晰显示底三张 / 上两张分组

### 💰 4D 赔率计算
- 支持三家彩票公司：**Magnum 4D · Sports Toto · Da Ma Cai**
- 投注方式：**Straight（直接号）** 和 **4A / iBox（任何顺序）**
- Big / Small 自由切换
- 4A 模式自动计算排列数（如 `1123` = 12 种），赔率按比例显示
- 实时显示各奖项可赢金额

### 📊 利息计算器
- **贷款**：输入金额 + 年利率 + 年限，自动算出每月还款、总利息，附逐月还款计划表
- **定期存款**：支持单利 / 复利，算出到期实收金额
- **民间借贷**：支持平息和利滚利（复利），清楚展示总利息

---

## 🛠 技术栈

- 纯 HTML + CSS + JavaScript，**零依赖，单文件**
- 千字图查询通过 [Vercel Serverless Python Proxy](https://github.com/junhong-623/vercel-proxy) 抓取 4dmanager.net
- 托管于 **GitHub Pages**（免费）

---

## 📁 项目结构

```
lucky-calc/
├── index.html    # 主文件（全部功能）
├── music.mp3     # 背景音乐（自行添加）
└── README.md
```

背景音乐需自行添加 `music.mp3`，推荐搜索「Chinese New Year ambient」或「casino lounge music」。  
免费素材：[pixabay.com/music](https://pixabay.com/music/)

---

## 🚀 部署方式

### GitHub Pages（当前）
1. Fork 或上传 `index.html` 到 GitHub repo
2. Settings → Pages → Branch: `main` → Save
3. 访问 `https://你的用户名.github.io/repo名/`

### Vercel Proxy（千字图查询）
千字图功能依赖独立的 proxy 服务，repo 在：  
👉 [github.com/junhong-623/vercel-proxy](https://github.com/junhong-623/vercel-proxy)

部署后在 `index.html` 顶部修改：
```js
const PROXY_URL = 'https://你的项目.vercel.app/api/search';
```

---

## 📌 注意事项

- 4D 赔率以官方公布为准，实际派彩可能因特别期数略有差异
- 千字图数据来源：4dmanager.net
- 本工具仅供参考娱乐，不构成任何投注建议

---

#### Test using Claude sample

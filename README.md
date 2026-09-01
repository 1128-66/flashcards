# 习思想 · 背诵抽认卡

在线访问：https://1128-66.github.io/flashcards/

## 目录结构

```
flashcards/
├── index.html          ← 首页（章节导航）
└── 习思想/
    ├── 00_导论_抽认卡.html
    ├── 01_第一章_抽认卡.html
    ├── …
    └── 17_第十七章_抽认卡.html
```

## 说明

- 每章一个独立 HTML，自包含、无外部依赖，进度存各设备浏览器本地（localStorage），各章互不干扰。
- 章节页顶部带「← 章节导航」返回首页链接。

## 如何新增/更新章节

1. 文件命名：`XX_第X章_抽认卡.html`（XX 为两位数字，决定首页排序）
2. 放入 `习思想/` 文件夹
3. 在章节页 `<header>` 标题上方保留返回链接（路径是 `../index.html`）：
   ```html
   <a class="home-link" href="../index.html">← 章节导航</a>
   ```
4. 推送后，在 `index.html` 的章节网格里复制一份 `<a class="chapter">…</a>` 卡片，改编号、标题、链接
5. `git add / commit / push origin main`，Pages 1~2 分钟自动生效

## 注意

- 仓库为公开仓库，链接不主动公开就不会被搜到，但请勿放入任何敏感信息。
- 章节文件名请不要包含空格。

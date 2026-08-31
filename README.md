# 背诵抽认卡（章节导航版）

在线访问：https://1128-66.github.io/flashcards/

## 这是什么

自包含的单文件 HTML 抽认卡合集，通过 GitHub Pages 部署，可在任意设备联网访问。学习进度保存在各设备浏览器本地（localStorage），不同设备间互不影响。

- **首页**（`index.html`）：章节导航，列出所有章节卡片
- **章节页**：每章一个独立 HTML，如 `01-导论.html`

## 如何新增一个章节

以新增「第二章」为例：

1. 制作好该章的抽认卡 HTML
2. 命名规范：`两位数字 + 连字符 + 章节名`，如 `02-xxx.html`（数字前缀决定首页排序）
3. 在章节页 `<header>` 的标题上方加返回入口（和 `01-导论.html` 里一致）：
   ```html
   <a class="home-link" href="index.html">← 章节导航</a>
   ```
4. 放入仓库并推送：
   ```bash
   git add 02-xxx.html
   git commit -m "新增第二章"
   git push origin main
   ```
5. **更新首页**：编辑 `index.html`，在「章节列表」注释之间复制一份 `<a class="chapter">…</a>`，把编号、标题、链接改好，再推送一次

推送后 GitHub Pages 会在 1~2 分钟内自动重新部署。

## 注意

- 仓库为公开仓库，链接不主动公开就不会被搜到，但请勿放入任何敏感信息。
- 章节文件名请保持英文数字前缀 + 中文名（如 `01-导论.html`），不要有空格。

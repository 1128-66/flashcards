# 导论 · 背诵抽认卡

在线访问：https://1128-66.github.io/flashcards/

## 这是什么

自包含的单文件 HTML 抽认卡（无任何外部依赖），通过 GitHub Pages 部署，可在任意设备（手机 / 平板 / 电脑）联网访问。学习进度保存在各设备浏览器本地（localStorage），不同设备间互不影响。

## 如何更新内容

在任意有 git 的电脑上：

```bash
git clone https://github.com/1128-66/flashcards.git
cd flashcards
# 用新的 HTML 覆盖 index.html
git add index.html
git commit -m "更新内容"
git push origin main
```

推送后 GitHub Pages 会在 1~2 分钟内自动重新部署，无需额外操作。

## 注意事项

- 仓库为公开仓库，链接不主动公开就不会被搜到，但请勿放入任何敏感信息。
- 更新时只需保持文件名为 `index.html`，否则访问地址会变化。

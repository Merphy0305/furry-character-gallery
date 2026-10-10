# Furry Character Gallery

一个用于整理、浏览和展示 Furry 角色图片的个人图库。

**🌐 在线画廊：[点击进入 Furry Character Gallery](https://merphy0305.github.io/furry-character-gallery/)**

## About

本项目是一个个人 Furry 角色图片图库，用于集中整理不同角色的图片与相关资料。

网站基于原生 HTML、CSS 和 JavaScript 构建，并通过 GitHub Pages 发布。角色信息与图片分开管理，图库数据由 GitHub Actions 自动生成，方便后续添加和整理内容。

## Features

- **Character Gallery** — 按角色分类展示图片。
- **Search** — 搜索角色名称及相关信息。
- **Tag Filtering** — 根据标签筛选角色。
- **Image Lightbox** — 放大查看图片，并在图片之间切换。
- **Automatic Gallery Generation** — 自动扫描角色目录并生成图库数据。
- **GitHub Pages** — 静态网站托管，无需独立服务器。

## Project Structure

```text
.
├── index.html
├── characters.json
├── gallery.json
├── <character-folder>/
└── .github/
    └── workflows/
        └── update-gallery.yml
```

| File / Directory | Description |
|---|---|
| `index.html` | 网站页面与前端逻辑 |
| `characters.json` | 手动维护的角色资料 |
| `gallery.json` | 自动生成的图库数据 |
| `<character-folder>/` | 各角色的图片目录 |
| `update-gallery.yml` | 自动生成图库数据的工作流 |

## Adding a Character

1. 在仓库根目录创建一个新的角色文件夹。
2. 将角色图片放入对应目录。
3. 在 `characters.json` 中添加角色名称、别名、简介和标签等信息。
4. 将修改提交到 `main` 分支。
5. 等待 GitHub Actions 自动更新 `gallery.json`，然后检查在线画廊。

支持的图片格式及具体处理规则请以当前工作流的实现为准。

## Technology

HTML · CSS · JavaScript · JSON · Python · GitHub Actions · GitHub Pages

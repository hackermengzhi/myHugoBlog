# Mengzhi Blog

Mengzhi 的个人博客，记录机器学习、编程实践与生活片段。站点基于 [Hugo](https://gohugo.io/) 和 [Hugo Theme Stack](https://github.com/CaiJimmy/hugo-theme-stack) 构建，并由 GitHub Actions 发布到 GitHub Pages。

在线访问：[hackermengzhi.github.io/myHugoBlog](https://hackermengzhi.github.io/myHugoBlog/)

## 本地运行

需要安装 Hugo Extended 和 Go：

```bash
hugo server --buildDrafts
```

访问终端输出的本地地址即可预览。生产构建使用：

```bash
hugo --gc --minify
```

## 内容结构

- `content/post/`：文章
- `content/page/pictures/`：图库及原图
- `data/music.json`：播放器歌单
- `layouts/`：首页、图库和自定义页脚交互
- `assets/scss/custom.scss`：站点视觉样式
- `config/_default/`：Hugo 与主题配置

推送到 `main` 或 `master` 分支后，`deploy.yml` 会自动构建并发布站点。

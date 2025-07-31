# borq minimal blog

一个极简、零构建的静态博客，灵感来自 [catherinejue.com]。

## 用法

1. 将仓库推送到 GitHub：
   - 新建仓库（名称可为 `your-username.github.io` 或任意名称）。
   - 推送本目录所有文件。

2. 启用 GitHub Pages：
   - 打开仓库 **Settings → Pages**，
   - Source 选择 **Deploy from a branch**，
   - Branch 选择 `main` 和根目录 `/`，保存。

3. 自定义域名（可选）：
   - 在 **Settings → Pages** 里填入你的域名，
   - 在域名 DNS 添加 `CNAME` 记录到 `your-username.github.io`。

## 写新文章

复制 `posts/hello.html` 为 `posts/your-slug.html`，修改标题、日期与正文。

> 如果更偏好用 Markdown 写作，可本地用任意工具（如 VS Code 插件、pandoc）导出为 HTML 粘贴到 `posts/`。

## 结构
```
.
├── 404.html
├── about.html
├── feed.xml
├── index.html
├── posts
│   ├── hello.html
│   └── notes-on-minimal-blogs.html
└── styles.css
```

## 设计原则

- 仅用原生 HTML + CSS，加载迅速且可长期维护；
- 页面宽度固定在 ~720px，聚焦文字；
- 链接下划线、浅色分隔线，保持视觉克制。


# borq.github.io
---
title: notes on building a minimal blog
date: 2025-07-30
description: 用最少的文件搭建一个可维护的静态博客
slug: notes-on-minimal-blogs
---

用最少的文件搭建一个可维护的静态博客：

1. **内容 Markdown 化**：写作体验更顺滑；
2. **构建脚本极简**：只用 Python 的 `markdown` + Jinja2；
3. **部署自动化**：Push → GitHub Actions → Pages。

> 保持 URL 结构为 `/posts/slug.html`，可随时迁移到任意静态站点生成器。

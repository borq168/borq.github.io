# borq minimal blog — Markdown 版

一个**Markdown 写作、自动构建、极简主题**的静态博客模板。

## 写作
- 在 `posts/` 里新建 `YYYY-MM-DD-slug.md`：
  ```md
  ---
  title: 文章标题
  date: 2025-07-31
  description: 简要描述
  slug: your-slug
  ---

  正文支持代码块、表格、引用等 Markdown 语法。
  ```
- 首页 / RSS 会自动生成；URL 固定为 `/posts/slug.html`。

## 配置
编辑 `site.yml`：站点名、签名、导航链接（work/other），以及 `base_url`（部署在子路径时填写）。

## 本地构建
```bash
pip install -r requirements.txt
python scripts/build.py
# 产物在 dist/，可用任意静态服务器预览
```

## GitHub Pages 部署
- 本仓库已包含 `.github/workflows/pages.yml`。推送到 `main` 分支后自动构建并发布到 Pages。
- 首次需在仓库 **Settings → Pages** 启用 `GitHub Actions` 作为发布源。

## 自定义域名
- 在 **Settings → Pages** 设置自定义域名；在 DNS 添加 CNAME 指向 `yourname.github.io`；(可选) 根目录添加 `CNAME` 文件避免被覆盖。

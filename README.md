# Shunxiang Liao 的个人主页

[![Deploy](https://github.com/Star1950625/Star1950625.github.io/actions/workflows/deploy.yml/badge.svg)](https://github.com/Star1950625/Star1950625.github.io/actions/workflows/deploy.yml)

🌐 **在线地址**: [https://star1950625.github.io](https://star1950625.github.io)

基于 [al-folio](https://github.com/alshedivat/al-folio) 主题构建的个人学术主页，托管于 GitHub Pages。

## 技术栈

- **框架**: Jekyll + Tailwind CSS
- **托管**: GitHub Pages（GitHub Actions 自动构建部署）
- **主题**: al-folio v1.x（运行时由独立版本化插件 gem 提供）

## 目录结构

```
_pages/           # 页面（about / blog / publications / projects / repositories / CV）
_posts/           # 博客文章（Markdown，文件名格式: YYYY-MM-DD-标题.md）
_projects/        # 项目展示（Markdown）
_bibliography/    # 论文列表（BibTeX，papers.bib）
_news/            # 主页新闻/公告
_data/            # 配置数据（社交链接、CV、repositories 列表）
assets/           # 图片、PDF 等静态资源
_includes/        # 本地覆盖的模板文件（head.liquid 追加自定义特效 CSS）
assets/css/custom.css  # 自定义样式（科技蓝绿主题、光晕、动画等特效）
```

## 如何更新

| 操作 | 方法 |
|------|------|
| 写博客 | 在 `_posts/` 新建 `YYYY-MM-DD-标题.md` |
| 加论文 | 在 `_bibliography/papers.bib` 添加 BibTeX 条目 |
| 加项目 | 在 `_projects/` 新建 `.md` 文件 |
| 展示仓库 | 编辑 `_data/repositories.yml` |
| 改社交链接 | 编辑 `_data/socials.yml` |
| 改头像 | 替换 `assets/img/prof_pic.jpg` |

修改后 push 到 `master` 分支，GitHub Actions 会自动构建并部署。

## 自定义特效

本站通过本地覆盖 `_includes/head.liquid` 注入了 `assets/css/custom.css`，实现了：
- 科技蓝绿主题色（亮色/暗色）
- 背景环境光晕
- 卡片悬浮效果
- 页面进入动画
- 渐变标题
- Inter / Space Grotesk / JetBrains Mono 字体

想调整颜色或动画，直接编辑 `assets/css/custom.css` 即可。

## License

本仓库内容版权归 [Shunxiang Liao](https://github.com/Star1950625) 所有。主题部分遵循 al-folio 的 MIT License。

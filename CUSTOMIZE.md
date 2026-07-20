# 主页填写指南

按下面顺序填写，通常 15–30 分钟即可完成个人化。

## 1. 首页资料

打开 `_pages/about.md`：

- `subtitle`：身份、实验室和学校，建议控制在一行。
- `profile.image`：头像文件名。将照片放到 `assets/img/` 后修改这里。
- `profile.more_info`：实验室、单位、城市、邮箱等照片下方信息。
- 正文前两段：建议写两段，每段 1–3 句。
- `interest-list`：建议保留 3–5 个短语。

照片推荐使用 4:5 竖版 JPG/WebP，至少 800×1000，文件小于 500 KB。将新照片放入
`assets/img/`，再更新 `profile.image` 即可。

## 2. 社交与学术链接（默认隐藏）

首页默认不显示社交与学术链接。若将来需要恢复，可在 `_data/socials.yml` 中填写链接，
并把首页的 `social` 设为 `true`。

## 3. Publications

论文保存在 `_bibliography/papers.bib`。每篇论文建议至少包含：

- `title`
- `author`
- `journal` 或 `booktitle`
- `year`
- `doi`
- `abbr`
- `bibtex_show = {true}`

设置 `selected = {true}` 的论文会显示在首页。当前精选了 3 篇第一作者论文。

## 4. Events

Events 页面中的每条动态对应内部 `_news/` 集合下一个 Markdown 文件。可复制现有文件并修改：

```yaml
---
layout: post
date: 2026-01-01
inline: true
related_posts: false
---
Your update here.
```

日期请使用 `YYYY-MM-DD`，网站会自动按时间倒序显示。

## 5. 主题样式

颜色、排版、卡片、响应式布局集中在 `assets/css/_academic.scss`。若只想换主题色，
修改其中浅色和深色模式下的 `--global-theme-color` 即可。

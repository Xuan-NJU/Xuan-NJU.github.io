# 主页填写指南

按下面顺序填写，通常 15–30 分钟即可完成个人化。

## 1. 首页资料

打开 `_pages/about.md`：

- `subtitle`：身份、实验室和学校，建议控制在一行。
- `profile.image`：头像文件名。将照片放到 `assets/img/` 后修改这里。
- `profile.more_info`：实验室、单位、城市、邮箱等右栏信息。
- 正文前两段：建议写两段，每段 1–3 句。
- `interest-list`：建议保留 3–5 个短语。

头像推荐使用竖版 JPG/WebP，至少 800×960，文件小于 500 KB。删除或替换
`assets/img/profile-placeholder.svg` 即可。

## 2. 社交与学术链接

打开 `_data/socials.yml`。GitHub、ORCID 和 Semantic Scholar 已填入；补充邮箱、
Google Scholar 或 LinkedIn 时，取消对应行的注释并填写值。

## 3. CV

打开 `_data/cv.yml`，替换所有 `EDIT` 或方括号占位内容。新增经历时复制相邻条目，
保持 YAML 缩进一致。

如果需要提供 PDF 下载：

1. 将文件命名为 `cv.pdf`，放入 `assets/pdf/`。
2. 在 `_pages/about.md` 的 `profile.more_info` 中添加 CV 链接。
3. 在 `_data/socials.yml` 取消 `cv_pdf` 一行的注释。

## 4. Publications

论文保存在 `_bibliography/papers.bib`。每篇论文建议至少包含：

- `title`
- `author`
- `journal` 或 `booktitle`
- `year`
- `doi`
- `abbr`
- `bibtex_show = {true}`

设置 `selected = {true}` 的论文会显示在首页。当前精选了 3 篇第一作者论文。

## 5. News

每条动态对应 `_news/` 下一个 Markdown 文件。可复制现有文件并修改：

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

## 6. 主题样式

颜色、排版、卡片、响应式布局集中在 `assets/css/_academic.scss`。若只想换主题色，
修改其中浅色和深色模式下的 `--global-theme-color` 即可。

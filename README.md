# Chengxuan Fu — Academic Homepage

这是为 `Xuan-NJU.github.io` 准备的学术主页源码，基于
[al-folio v1.x](https://github.com/alshedivat/al-folio)，并参考
[xutangzhi.github.io](https://xutangzhi.github.io/) 的克制型学术排版。

网站只保留三个英文内容栏目：Home、Publications、Events。支持跟随系统、日间、
夜间三种配色，兼容移动端布局、BibTeX 自动排版和 GitHub Pages 自动部署。

## 最常修改的文件

| 内容                           | 文件                       |
| ------------------------------ | -------------------------- |
| 姓名、网址、站点描述           | `_config.yml`              |
| 首页身份、头像、简介、研究方向 | `_pages/about.md`          |
| GitHub、ORCID、邮箱等链接      | `_data/socials.yml`        |
| 论文列表                       | `_bibliography/papers.bib` |
| Events                         | `_news/*.md`               |

完整填写说明见 [CUSTOMIZE.md](CUSTOMIZE.md)，上线步骤见 [DEPLOY.md](DEPLOY.md)。

## 当前论文数据

已收录并交叉核验 Chengxuan Fu 自 2024 年起的 6 篇正式出版物；当前未检索到
2024 年条目。数据核对时间为 2026-07-18，来源包括 DOI/Crossref、IEEE、ACM、
DBLP、ORCID 和 Semantic Scholar。

## 模板基线与覆盖

- al-folio starter：`main`，参考提交 `d755f8dec78ad90d39d0517b13e752ee8f887613`
- al_folio_core：`1.0.11`
- 本站有两个有意保留的主题样式文件：`assets/css/main.scss`、
  `assets/css/_academic.scss`

升级 al-folio 后，请重点检查这两个文件与新版主题的兼容性。

## License

This project retains the upstream al-folio MIT license. See [LICENSE](LICENSE).

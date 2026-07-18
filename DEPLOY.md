# 部署到 GitHub Pages

## 1. 创建仓库

在 GitHub 创建一个公开仓库，名称必须为：

```text
Xuan-NJU.github.io
```

不要额外创建 README、License 或 `.gitignore`，然后把本目录的全部内容推送到
仓库的 `main` 分支。

## 2. 允许自动部署

进入仓库：

1. `Settings → Actions → General`
2. 在 `Workflow permissions` 选择 `Read and write permissions`
3. 保存设置

随后进入 `Actions`，手动运行一次 `Deploy site`，或向 `main` 推送一次修改。

## 3. 设置 Pages 来源

第一次部署任务成功后，仓库会出现 `gh-pages` 分支。进入：

1. `Settings → Pages`
2. Source 选择 `Deploy from a branch`
3. Branch 选择 `gh-pages`
4. Folder 选择 `/(root)`
5. 保存

网站地址将是：<https://xuan-nju.github.io/>。

## 常见问题

- 页面没有样式：确认 `_config.yml` 中 `url` 是 `https://xuan-nju.github.io`，
  且 `baseurl` 为空。
- Action 无法推送：确认 Workflow permissions 为读写权限，且 `gh-pages` 没有阻止
  Action 推送的分支保护。
- 只改 README 没有触发：手动运行 `Deploy site`，或同时修改一个内容/配置文件。
- 不要把 Pages 来源设成 `main`；本站需要 al-folio 的完整构建流程。

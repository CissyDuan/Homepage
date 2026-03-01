# 在线发布（GitHub Pages）

本项目已包含自动部署工作流：
- `.github/workflows/deploy-pages.yml`

## 你需要做的事

1. 把当前目录推送到 GitHub 仓库（默认分支建议为 `main`）。
2. 在仓库中打开：`Settings -> Pages`
3. 在 `Build and deployment` 中选择：`Source = GitHub Actions`
4. 推送一次代码后，等待 `Actions` 里的 `Deploy static site to GitHub Pages` 运行成功。

## 访问地址

发布成功后，网站地址通常是：
- `https://<你的GitHub用户名>.github.io/<仓库名>/`

## 注意

- `网站内容.xlsx`、`网站内容_英文.xlsx`、所有图片/PDF 必须和 `index.html` 一起提交到仓库根目录。
- 如果你仓库名不是 `<用户名>.github.io`，建议后续把 `script.js` 里读取路径改成基于当前目录的相对路径（当前版本已是相对路径，通常可直接用）。

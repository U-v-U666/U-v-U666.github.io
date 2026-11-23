# Luyuan Jiang 的个人主页

网址：<https://u-v-u666.github.io/>

这是一个无需安装依赖或构建的静态网站。

- `index.html`：首页内容、布局和样式。
- `favicon.svg`：浏览器标签页图标。
- `.nojekyll`：让 GitHub Pages 直接发布静态文件。

## 本地预览

在仓库目录中运行：

```powershell
python -m http.server 8000 --bind 127.0.0.1
```

然后访问 <http://127.0.0.1:8000>。按 `Ctrl+C` 停止预览。

## 更新网站

编辑 `index.html` 后提交并推送到 `main` 分支，GitHub Pages 会自动更新：

```powershell
git add index.html favicon.svg README.md .nojekyll
git commit -m "Update homepage"
git push origin main
```

发布设置：仓库 **Settings → Pages → Deploy from a branch → main → / (root)**。

仓库名 `U-v-U666.github.io` 与 GitHub 账号一致，因此网站直接发布在 `https://u-v-u666.github.io/`，不包含项目路径，也无需配置自定义域名或 DNS。

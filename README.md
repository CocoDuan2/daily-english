# daily-english

日常亲子英语静态网站，按生活主题浏览场景对话，包含英语、音标、中文和长图。

## 在线访问

https://cocoduan2.github.io/daily-english/

## 项目结构

- `index.html`：首页
- `themes.html`、`themes/`：主题列表和主题详情
- `mine.html`：学习进度
- `pages/`：场景对话页面
- `images/`：场景长图
- `data/`：场景源数据

## 部署与更新

GitHub Pages 从 `main` 分支的根目录发布。`.nojekyll` 表示直接发布静态文件，无需 Jekyll 构建。

新增或修改场景后，在项目目录运行：

```sh
git add index.html themes.html mine.html pages/ themes/ images/ data/
git commit -m "Update daily English scenes"
git push origin main
```

首次发布需要在仓库 Settings → Pages 中启用 `Deploy from a branch`，选择 `main` 和 `/ (root)`。

## 说明

- 学习进度保存在当前浏览器的 `localStorage` 中，不上传、不跨设备同步。
- 网站及已提交的源数据对外公开，请勿放入个人隐私或密钥。
- 本地备份和临时锁文件通过 `.gitignore` 排除，不上传到仓库。

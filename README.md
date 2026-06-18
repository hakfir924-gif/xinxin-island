# 鑫鑫充电站 - Vercel 静态部署版

这是一个纯静态项目，只有 HTML、CSS 和 JavaScript，不需要后端服务。

## 文件说明

- `index.html`：首页，包含全部页面、样式和交互逻辑。
- `vercel.json`：Vercel 静态站点配置。

## 部署步骤

### 方法一：通过 GitHub Pages 部署

1. 新建一个 GitHub 仓库。
2. 把本文件夹里的 `index.html`、`README.md`、`vercel.json` 上传到仓库根目录。
3. 进入仓库的 `Settings`。
4. 打开 `Pages`。
5. Source 选择 `Deploy from a branch`。
6. Branch 选择 `main`，目录选择 `/root`。
7. 保存后等待 GitHub Pages 生成访问地址。

### 方法二：通过 Vercel 网页部署

1. 打开 [Vercel](https://vercel.com/) 并登录。
2. 新建一个 GitHub 仓库，把本文件夹里的文件上传进去。
3. 在 Vercel 点击 `Add New...`，选择 `Project`。
4. 选择刚才的仓库。
5. Framework Preset 选择 `Other`。
6. Build Command 留空。
7. Output Directory 留空。
8. 点击 `Deploy`。

### 方法三：通过 Vercel CLI 部署

1. 进入本文件夹。
2. 执行 `vercel`。
3. 按提示登录并确认项目设置。
4. 如果要发布正式版本，执行 `vercel --prod`。

## 检查清单

- 首页路径是 `/index.html`，部署后访问域名根路径即可打开。
- 页面没有外部图片资源，动物使用 emoji 表示，不会出现图片路径丢失。
- 按钮都是页面内 JavaScript 交互，不依赖跳转路径。
- 已加入手机端和微信浏览器友好的视口、安全区、触控按钮样式。
- 所有数据保存在浏览器本地，不需要后端和数据库。

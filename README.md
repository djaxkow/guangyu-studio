# 工作室展示网站

一个现代化的工作室展示单页网站，采用响应式设计，支持桌面端和移动端。

## 功能特点

- 🎨 现代简约设计风格
- 📱 完全响应式，适配各种设备
- ✨ 流畅的动画效果
- 🔍 作品分类筛选
- 📊 数字计数动画
- 📝 联系表单
- 🚀 平滑滚动导航
- ⬆️ 返回顶部按钮

## 网站结构

1. **首页英雄区** - 工作室名称和标语
2. **关于我们** - 工作室简介和数据统计
3. **服务项目** - 提供的6项服务
4. **作品展示** - 作品集，支持分类筛选
5. **团队介绍** - 核心成员展示
6. **联系我们** - 联系方式和表单
7. **页脚** - 导航链接和社交媒体

## 文件说明

- `index.html` - 主页面
- `style.css` - 样式文件
- `script.js` - 交互脚本

## 部署到 GitHub Pages

### 方法一：通过 GitHub 网页界面（推荐新手）

1. 登录你的 GitHub 账号
2. 点击右上角 "+" → "New repository"
3. 仓库名称建议用：`你的用户名.github.io`（这样访问地址就是 `https://你的用户名.github.io`）
   - 或者任意名称，比如 `studio-website`（访问地址就是 `https://你的用户名.github.io/studio-website`）
4. 选择 "Public"，勾选 "Add a README file"
5. 点击 "Create repository"
6. 进入仓库后，点击 "Add file" → "Upload files"
7. 把 `index.html`、`style.css`、`script.js` 三个文件拖进去
8. 点击底部 "Commit changes"
9. 然后点击仓库的 "Settings" → 左侧找到 "Pages"
10. 在 "Build and deployment" 下，Source 选择 "Deploy from a branch"
11. Branch 选择 `main` 或 `master`，文件夹选择 `/ (root)`
12. 点击 "Save"
13. 等待几分钟，网站就可以通过 GitHub 提供的链接访问了！

### 方法二：通过 Git 命令行

```bash
# 1. 初始化仓库
git init

# 2. 添加文件
git add .

# 3. 提交
git commit -m "Initial commit"

# 4. 添加远程仓库（替换为你的仓库地址）
git remote add origin https://github.com/你的用户名/仓库名.git

# 5. 推送
git branch -M main
git push -u origin main
```

然后在仓库设置中开启 GitHub Pages 即可。

## 自定义修改

### 修改工作室名称
打开 `index.html`，搜索 "STUDIO" 和 "创意工作室"，替换成你的工作室名称。

### 修改内容
- 关于我们的文字：在 `index.html` 中找到 `<section id="about">` 部分修改
- 服务项目：找到 `<section id="services">` 修改
- 作品展示：找到 `<section id="works">` 修改
- 团队成员：找到 `<section id="team">` 修改
- 联系方式：找到 `<section id="contact">` 修改

### 修改颜色主题
打开 `style.css`，找到 `:root` 部分，修改 `--primary-color` 等颜色变量。

### 替换图片
目前图片位置用渐变色块占位，你可以：
1. 把图片文件放到同一目录下
2. 在 `index.html` 中找到对应的位置，把 `<div class="xxx">` 替换成 `<img src="图片文件名.jpg" alt="描述">`
3. 在 `style.css` 中调整对应的样式

## 技术栈

- HTML5
- CSS3（Grid + Flexbox 布局）
- 原生 JavaScript（无依赖）
- Google Fonts（Noto Sans SC）

## 浏览器兼容性

支持所有现代浏览器：
- Chrome
- Firefox
- Safari
- Edge

## 许可证

MIT License

# GitHub Pages 开启教程

把你的 GitHub 仓库变成一个任何人都能访问的网站，不需要服务器、不需要域名、不需要懂代码。

## 前提

- 已有 GitHub 账号
- 已创建一个仓库，且仓库中有 `README.md`

## 步骤

### 1. 进入仓库设置

打开你的仓库页面，点击右上角的 **Settings**（设置）。

### 2. 找到 Pages

在左侧菜单中找到 **Pages** 选项。

### 3. 配置来源

- **Source** 选择 `Deploy from a branch`
- **Branch** 选择 `main`（或你的默认分支）
- **Folder** 选择 `/ (root)`
- 点击 **Save**

### 4. 等待部署

保存后，GitHub 会自动构建你的网站。通常需要 1-3 分钟。

页面顶部会显示你的网站地址（以本仓库为例）：

```
https://sharronxue.github.io/ai-toolbox/
```

格式规律：`https://用户名.github.io/仓库名/`

### 5. 验证

在浏览器中打开这个地址，你应该能看到 README.md 的渲染内容。

## 常见问题

| 问题 | 解决方案 |
|------|---------|
| 打开是 404 | 等几分钟再试；确认分支选对了 |
| 样式不对 | 确认仓库是 Public（公开的） |
| 想用自定义域名 | 在 Pages 设置页的 Custom domain 中填入你的域名，然后在域名 DNS 中添加 CNAME 记录指向 `sharronxue.github.io` |

## 进阶：用 Jekyll 主题

GitHub Pages 默认使用 Jekyll 引擎。你可以在仓库根目录创建 `_config.yml` 来配置主题：

```yaml
theme: jekyll-theme-minimal
title: AI 工具箱
description: 个人 AI 工具使用技巧与提示词分享
```

保存后推送，GitHub 会自动应用主题。

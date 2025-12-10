# GitHub 上传指南 / GitHub Upload Guide

## 快速上传步骤 / Quick Upload Steps

### 方法一：使用 GitHub Desktop（推荐）

1. 下载并安装 [GitHub Desktop](https://desktop.github.com/)
2. 打开 GitHub Desktop
3. 点击 "File" > "Add Local Repository"
4. 选择这个文件夹：`/Users/liyunuo/Desktop/Harmonic-collection-project/Home/entery1`
5. 点击 "Publish repository" 按钮
6. 输入仓库名称，选择是否公开，然后点击 "Publish"

### 方法二：使用命令行 / Using Command Line

#### 1. 打开终端 / Open Terminal

按 `Cmd + Space`，输入 "Terminal"，然后回车

#### 2. 进入项目目录 / Navigate to project directory

```bash
cd /Users/liyunuo/Desktop/Harmonic-collection-project/Home/entery1
```

#### 3. 初始化 Git 仓库 / Initialize Git repository

```bash
git init
```

#### 4. 添加所有文件 / Add all files

```bash
git add .
```

#### 5. 创建提交 / Create commit

```bash
git commit -m "Initial commit: Harmonic Collection cocktail website"
```

#### 6. 在 GitHub 上创建新仓库 / Create new repository on GitHub

- 访问 https://github.com/new
- 输入仓库名称（推荐：`harmonic_collection_cocktail_menu`）
- 选择公开或私有
- **不要**勾选 "Initialize this repository with a README"
- 点击 "Create repository"

#### 7. 添加远程仓库 / Add remote repository

将 `YOUR_USERNAME` 和 `YOUR_REPO_NAME` 替换为你的实际信息：

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
```

#### 8. 推送到 GitHub / Push to GitHub

```bash
git branch -M main
git push -u origin main
```

### 如果遇到问题 / Troubleshooting

#### 首次使用 Git 需要配置 / First time Git setup

```bash
git config --global user.name "你的名字"
git config --global user.email "your.email@example.com"
```

#### 如果提示需要安装 Xcode 命令行工具 / If Xcode command line tools needed

在终端运行：
```bash
xcode-select --install
```

然后按照提示完成安装。

#### 如果已经存在远程仓库 / If remote repository already exists

```bash
git remote remove origin
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

## 文件说明 / File Description

- `.gitignore` - Git 忽略文件配置（已创建）
- `README.md` - 项目说明文档（已创建）
- 所有 HTML、CSS、JavaScript 和图片文件都已准备好上传

## 完成！/ Done!

上传完成后，你的网站文件将在 GitHub 上可见。如果需要使用 GitHub Pages 托管网站，可以在仓库设置中启用。


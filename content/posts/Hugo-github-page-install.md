+++
date = '2026-09-10T09:09:34+08:00'
title = 'Hugo Github Page Install'
categories = ['建站']
tags = ['Hugo', 'GitHub Pages', 'PaperMod']
+++


# Hugo github page install
- [Hugo Quick start](https://gohugo.io/getting-started/quick-start/)
- [Theme: PaperMod](https://github.com/adityatelange/hugo-PaperMod)


## 安装

1. 初始化项目
```shell
hugo new project yu-xiaoyao.github.io
cd yu-xiaoyao.github.io
git init

git branch -M main
```

2. 安装主题 
```shell
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)


# if update the theme
git submodule update --remote --merge


echo "theme = 'PaperMod'" >> hugo.toml

hugo server

```

## 添加文章内容
```shell
hugo new content content/posts/Hugo-github-page-install.md
```
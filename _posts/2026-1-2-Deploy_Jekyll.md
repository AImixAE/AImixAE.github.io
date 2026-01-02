---
title: 部署 Jekyll
description: 并且带有好看的主题(✧∀✧)
author: AImixAE Nya Mocha
date: 2026-1-2 08:00:00 +0800
categories: [Blog, 技术]
tags: [blog]
image:
    path: /assets/img/posts/2026-1-2-Deploy_Jekyll/p0.png
---

# 部署 带有 Chirpy 主题的 Jekyll

想知道像我这样好看的 Blog 是怎么搭建的嘛? 来看看这个吧喵!

## 创建项目

我们要先登录 github,
 随后再来到 [Chirpy-Starter](https://github.com/cotes2020/chirpy-starter) 项目.

点击 <kbd>Use this template</kbd> 按钮后选择 <kbd>Create a new repository</kbd>.

将仓库命名为 `<username>.github.io` 或者其他名字.

> 提示: 记得将 `<username>` 修改为你的 github 用户名
{: .prompt-tip }

我们就大功告成了!

## 配置本地环境 _(可选)_

我们既可以创建本地的环境以便我们调试, 也可以无所畏惧提交给 github.

我们有两种方式来搭建

### 使用开发容器 _(推荐用于 **Windows**)_

这种方式可以隔离我们的系统, 防止一些冲突, 并且也方便我们管理.

1. 安装 **Docker**
    - 在 **Windows/MacOS** 上, 我们可以安装 [Docker Desktop](https://www.docker.com/products/docker-desktop/)
    - 在 **Linux** 上, 我们更推荐使用包管理器安装
        - **Arch Linux**: `sudo pacman -S docker`
        - **其他发行版**: 按照自己所使用的包管理器去安装 [_Docker Engine_](https://www.docker.com/products/docker-desktop)
2. 安装 [**Visual Studio Code**](https://code.visualstudio.com) 和 **Dev Containers 扩展**
3. 克隆你的 Repo _(需要 `git`)_

_(详细见 [Getting Started - Use dev containers](https://chirpy.cotes.page/posts/getting-started/#using-dev-containers-recommended-for-windows))_

随后等待设置完成就可以了喵

### 本地安装

首先, 我们要下载 [**Ruby**](https://www.ruby-lang.org/zh_cn/downloads) 并确保还有 `bundle`

再克隆你的 Repo

随后在仓库根目录运行 `bundle` 来安装依赖

## 使用

既然安装好了环境, 我们就可以本地运行测试

```bash
bundle exec jekyll serve
```

随后访问 <http://127.0.0.1:4000> 就可以了喵

## 配置

这是我们自己的 Blog, 所以当然要配置啦~

我们需要编辑 `_config.yml`

## 中文

因为使用 **chirpy-starter**, 所以没有很多内容 _(包括语言)_

所以我们要到 [jekyll-theme-chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) 获取一份 `_data/locales` 并复制到自己项目下

随后编辑 `_config.yml` 并将 `lang` 的值修改为 `zh-CN`

## 部署 _(Github Actions)_

我们可以 `git push` 到 Github 上, 利用 github pages 和 github actions 来配置自己的 blog

如果仓库名字为 `<username>.github.io`, 那么不需要动, 但如果使用的其他名字, 请到 Settings 配置 Pages

随后就可以访问了

## 手动构建

我们可以构建一个静态网页供我们自己的服务器使用

```bash
JEKYLL_ENV=production bundle exec jekyll b
```

随后就会放到 `_site` 文件夹中

## 已知问题

不知道为什么, 在电脑端上的代码块显示会有 bug, 但移动端没有.

如果你有其他问题, 欢迎在下面讨论喵!

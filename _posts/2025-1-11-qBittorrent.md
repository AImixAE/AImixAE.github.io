---
title: qBittorrent 使用
description: This is my first blog.
author: AImixAE
date: 2025-1-11 14:00:00 +0800
categories: [Blog, Temp]
tags: [blog]
image:
    path: /assets/img/posts/2025-1-11-qBittorrent/St1.png
---

# qBittorrent 使用

网上不知何时起，出现了一堆*无限下载*的 `BT客户端`

他们的行为被称之为 **吸血**

> 简解 **吸血**
>
> 由于用户上传带宽比企业上传带宽更便宜，因此企业就想利用用户的带宽来减轻自己带宽的消耗
>
> 于是早期企业就与用户 "合伙" *(`PCDN`)*
>
> 但是这样运营商就会吃亏，因此他们就想办法封禁这种行为
>
> 但是这样还是防不住他们，于是企业就弄了一些特殊的 `BT客户端`，以此共享用户们的带宽
>
> 这样就造成了 **吸血**

那么，如何在 `Arch Linux` 避免 **吸血** 呢?

那就是要介绍的 `qBittorrent` 了

## 安装

```bash
sudo pacman -S qbittorrent-enhanced-git # 在 archlinuxcn 源里安装
paru -S qbittorrent-enhanced-git # 在 AUR 里安装
```

![St1.png](/assets/img/posts/2025-1-11-qBittorrent/St1.png)

## 配置

我们进入 [文档](https://docs.qq.com/doc/DQnJBTGJjSFZBR2JW) 找到 `对策A2`

*或者是这个*:

```plaintext
-GT0003- github.com/anacrolix/torrent\s\(devel\)\s\(anacrolix/torrent\sunknown\)
-DT0001- .*
-HP0001- .*
-XM0001- .*
.* Gopeed dev
```

把上面的内容写到 `~/.local/share/qBittorrent/peer_blacklist.txt` 里

再找到 `对策B`

然后在 `~/.local/share/qBittorrent` 里创建一个 `.dat` 文件

然后把 `ip` 全部复制进去，如果多了一行空白，请删掉

## In the end

最后，我们可以用 `qBittorrent` 下载各种资源了

也不用担心 **吸血** 了🥳

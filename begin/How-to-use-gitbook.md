---
description: 一个很简短的 gitbook 使用介绍
---

> 目前 Gitbook 使用 Shwvi 账号部署，若以后有需求，可以很简单地迁移到社团的公用账号部署

## 什么是 Gitbook

Gitbook 是一个非常适合开发者管理文档的平台，因为它可以绑定你的 GitHub repo，并且提供了很简单易用的方式
去组织你的文章结构。

Gitbook 支持富文本编辑器，但是我们主要使用 markdown 进行编辑，利用 Git 进行协作。

## Gitbook 基本使用方法

使用 Gitbook 就如同你写代码一样，你只需要和其他人一起协作完成 Gitbook 对应的 repo 即可

首先，克隆仓库到本地

```
git clone https://github.com/NJU-NOVA/web-doc.git
```

然后，对里面的内容进行更改，并将更改 push 到远程的仓库，gitbook 将自动完成同步（可能需要几分钟时间）

你的一般使用形式如下：

```
git add .
git commit -m "my changes"
git push -u origin master
```

### 目录管理

在 Gitbook 的 repo 中，你会看到根目录下有一个 `SUMMARY.md` 的文档，
此文档会有如下的结构：

```markdown
# Table of contents

- [Nova 前端组](README.md)

## 开始

- [如何使用 Gitbook](/begin/How-to-use-gitbook.md)

## 学习路线

- [基础](/learning-path/readme.md)
  - [eg1]()

## 前端活动记录

- [In 2021]()
  - [Week 6](/record/Week6.md)
```

其实你可以通过这个结构一瞥 gitbook 的目录组织形式

你可以使用 `##` `###` 等定义直接显示在侧边栏的目录

同时，使用无序列表和链接定义目录结构和对应文章，不同缩进的无序列表则代表了目录层次，
从网站的显示效果，你可以很容易明白这样的效果

### 内容编辑

如前所叙，我们通常使用 markdown 进行文档编辑，所以和你平常写 markdown 是一样的

如果你不知道如何使用 markdown，请看[markdown 简易教程](../utils/how-to-use-markdown.md)

## 为什么要使用 Gitbook

1. 方便地使用 Git 进行合作
2. 使用方式足够简单易用
3. 使用方式更符合程序员习惯
4. 免费部署，可安心部署到公网访问

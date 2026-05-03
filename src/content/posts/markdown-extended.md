---
title: Markdown 扩展功能
published: 2024-05-01
updated: 2024-11-29
description: '了解 Fuwari 中更多 Markdown 功能。'
image: ''
tags: [演示, 示例, Markdown, Fuwari]
category: '示例'
draft: false 
---

## GitHub 仓库卡片
你可以添加链接到 GitHub 仓库的动态卡片，页面加载时会从 GitHub API 拉取仓库信息。 

::github{repo="Kolandaina/fuwari-blog"}

使用 `::github{repo="<owner>/<repo>"}` 这段代码可以创建一个 GitHub 仓库卡片。

```markdown
::github{repo="Kolandaina/fuwari-blog"}
```

## 提示块

支持以下几种提示块类型：`note` `tip` `important` `warning` `caution`

:::note
突出显示用户即使快速浏览也应该注意的信息。
:::

:::tip
有助于用户更顺利完成操作的可选信息。
:::

:::important
帮助用户成功完成操作所必需的关键信息。
:::

:::warning
由于存在潜在风险，需要用户立即注意的关键内容。
:::

:::caution
某个操作可能带来的负面后果。
:::

### 基本语法

```markdown
:::note
突出显示用户即使快速浏览也应该注意的信息。
:::

:::tip
有助于用户更顺利完成操作的可选信息。
:::
```

### 自定义标题

提示块的标题可以自定义。

:::note[MY CUSTOM TITLE]
这是一个带自定义标题的提示。
:::

```markdown
:::note[MY CUSTOM TITLE]
This is a note with a custom title.
:::
```

### GitHub 语法

> [!TIP]
> 也支持 [GitHub 语法](https://github.com/orgs/community/discussions/16925)。

```
> [!NOTE]
> The GitHub syntax is also supported.

> [!TIP]
> The GitHub syntax is also supported.
```

### 剧透内容

你可以在文本中添加剧透内容。这里同样支持 **Markdown** 语法。

内容 :spoiler[被隐藏了 **ayyy**]！

```markdown
内容 :spoiler[被隐藏了 **ayyy**]！

```
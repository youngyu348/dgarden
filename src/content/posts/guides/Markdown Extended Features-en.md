---
title: Markdown Extended Features
published: 2025-04-25
tags:
  - Guide
toc: false
lang: en
abbrlink: markdown-extended-features
---

Here are some extended Markdown features supported by Retypeset, including syntax examples and their stylistic effects.

## Figure Captions

To create automatic figure captions, use the standard Markdown image syntax `![alt](src)`. To hide the caption, add an underscore `_` before the `alt` text or leave the `alt` text empty.

### Syntax

```
![Image description](./full/or/relative/path/of/image)

![_Image description](./full/or/relative/path/of/image)
```

### Output

![Image description](https://image.radishzz.cc/image/gallery/06.webp)

![_Image description](https://image.radishzz.cc/image/gallery/06.webp)

## Github Repository Cards

To create a Github repository card, use the double colon syntax `::github{repo="owner/repo"}`. Repository data is fetched from the GitHub API after the page loads.

### Syntax

```
::github{repo="radishzzz/astro-theme-retypeset"}
```

### Output

::github{repo="radishzzz/astro-theme-retypeset"}

## Admonition

To create admonition blocks, use the GitHub syntax `> [!TYPE]` or the triple colon syntax `:::type`. Following types are supported: `note`, `tip`, `important`, `warning`, and `caution`.

### Syntax

```
> [!NOTE]
> Useful information that users should know, even when skimming content.

:::note
Useful information that users should know, even when skimming content.
:::

:::note[YOUR CUSTOM TITLE]
This is a note with a custom title.
:::
```

### Output

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

:::warning
Urgent info that needs immediate user attention to avoid problems.
:::

:::caution
Advises about risks or negative outcomes of certain actions.
:::

:::note[YOUR CUSTOM TITLE]
This is a note with a custom title.
:::

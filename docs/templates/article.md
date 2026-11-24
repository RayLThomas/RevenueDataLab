---
title: Article title
description: One or two sentence summary.
date: 2025-01-01
categories: # optional; any values work. Related articles share a category.
  - Data Engineering # also: SQL & Databases, Python, AI & Automation, Revenue Operations, Business Intelligence, CRM Architecture
tags: # optional
  - example
author: Author Name # optional; defaults to authorName in src/_data/site.json
authorLinkedin: https://www.linkedin.com/in/your-profile/ # optional
image: /images/articles/article-slug.png # optional; use a 16:9 image that follows ../ARTICLE-IMAGE-STYLE.md
imageAlt: Describe the image # required when image is set; omit both fields to use the standard card fallback
readingTime: 5 # optional; calculated automatically if omitted
draft: true # remove or set false to publish
---

Write in Markdown. Fenced code blocks are highlighted at build time:

Featured images should follow [`docs/ARTICLE-IMAGE-STYLE.md`](../ARTICLE-IMAGE-STYLE.md). Use a 16:9 source image, store it under `src/images/articles/`, and provide useful alternative text. Article cards automatically use the standard branded fallback when `image` is omitted.

```sql
SELECT 1;
```

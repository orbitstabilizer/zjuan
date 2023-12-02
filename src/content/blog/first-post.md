---
author: Yusuf AKIN
pubDatetime: 2023-12-03T03:01:30Z
title: First Post
postSlug: first-post
featured: true
draft: false
tags:
  - test
description:
    First post.
---

First post.

## Table of contents

## Frontmatter

Frontmatter is the main place to store some important information about the blog post (article). Frontmatter lies at the top of the article and is written in YAML format. Read more about frontmatter and its usage in [astro documentation](https://docs.astro.build/en/guides/markdown-content/).

Here is the list of frontmatter property for each post.

| Property           | Description                                                                     | Remark                                        |
| ------------------ | ------------------------------------------------------------------------------- | --------------------------------------------- |
| **_title_**        | Title of the post. (h1)                                                         | required<sup>\*</sup>                         |
| **_description_**  | Description of the post. Used in post excerpt and site description of the post. | required<sup>\*</sup>                         |
| **_pubDatetime_**  | Published datetime in ISO 8601 format.                                          | required<sup>\*</sup>                         |
| **_author_**       | Author of the post.                                                             | default = SITE.author                         |
| **_postSlug_**     | Slug for the post. Will automatically be slugified.                             | default = slugified title                     |
| **_featured_**     | Whether or not display this post in featured section of home page               | default = false                               |
| **_draft_**        | Mark this post 'unpublished'.                                                   | default = false                               |
| **_tags_**         | Related keywords for this post. Written in array yaml format.                   | default = others                              |
| **_ogImage_**      | OG image of the post. Useful for social media sharing and SEO.                  | default = SITE.ogImage or generated OG image  |
| **_canonicalURL_** | Canonical URL (absolute), in case the article already exists on other source.   | default = `Astro.site` + `Astro.url.pathname` |

Only `title`, `description` and `pubDatetime` fields in frontmatter must be specified.

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A Jekyll documentation site for the UCLA Library Data Science Center, built with the [Just the Docs](https://just-the-docs.github.io/just-the-docs/) theme (v0.12.0) and published to GitHub Pages. Content is Markdown; no JavaScript framework involved.

Live site: https://ucla-data-science-center.github.io/docs/

## Commands

```bash
bundle install               # install gems (first time or after Gemfile changes)
bundle exec jekyll serve     # local preview at http://localhost:4000
bundle exec jekyll build     # production build to ./_site
```

CI runs `bundle exec jekyll build` on every PR. Deployment to Pages triggers on push to `main`.

## Content structure

All documentation lives under `docs/`. Top-level sections:

| Directory | Content |
|---|---|
| `docs/handbook/` | DataSquad Handbook (staff-facing operational guide) |
| `docs/dataverse/` | UCLA Dataverse user documentation |
| `docs/policies/` | Code of conduct, collection policy, preservation, ToS |
| `docs/faq/` | FAQ index |
| `docs/get_started/` | Quick-start guides |
| `docs/datasquad-website-guide/` | How-to for the DataSquad Astro website |

## Navigation and frontmatter

Just the Docs drives navigation entirely from frontmatter. Every page needs:

```yaml
---
title: Page Title
layout: default        # use "home" only for index.md
nav_order: N           # integer controls sidebar order within a section
parent: Section Title  # must match the `title` of the parent page exactly
has_children: true     # required on section index pages
---
```

Omit `parent` for top-level sections. Sidebar ordering is controlled by `nav_order` on each page, not by filenames or directory order.

## Adding or editing pages

- Drop new `.md` files into the appropriate `docs/` subdirectory.
- Set frontmatter as above; the sidebar updates automatically.
- Filenames use lowercase with hyphens or underscores (existing convention is mixed - match the section you're working in).
- Internal links should use `{{ site.baseurl }}/path/to/page.html` for reliability across environments.
- Images go in `assets/` and reference via `{{ site.baseurl }}/assets/...`.

## Site configuration

`_config.yml` sets the theme, title, and `url`. The `_includes/head_custom.html` injects a custom favicon. Do not change `url` without also updating the GitHub Pages settings.

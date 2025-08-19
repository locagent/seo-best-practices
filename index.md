---
layout: default
title: "Building Global Apps - An SEO Guide"
description: "SEO best practices for vibe coding MVPs built with Lovable, Bubble, Bolt, Replit, v0, Floot, Cursor, Windsurf, Claude Code, etc. AI app builders."
---

# Building Global AI Apps: An SEO Guide

## Table of Contents

1. [Infrastructure](#infrastructure)
2. [Best Practices](#best-practices)
3. [Code Review](#code-review)
4. [Checklist](#checklist)

---

## Infrastructure

### 1. Head Tags
- Every indexable page needs a unique, descriptive `<title>` and a helpful meta description.

### 2. Robots Rules
- Use `robots.txt` only to manage crawling pressure. Don’t use it to keep pages out of search engines (use `noindex` or authentication). Place robots at the site root.

### 3. Sitemap
- Maintain a sitemap with the domain.

### 4. URL Structure
- Keep URLs simple, readable, and stable. Avoid duplicate parameter variants. Prefer one canonical URL per page.

### 5. Sitemaps
- Provide an XML sitemap listing canonical URLs, link it in robots.txt.

### 6. Structured Data
- Add JSON-LD structured data using Schema.org to enhance understanding and eligibility for rich results.

### 7. Errors
- Ship a helpful `/404.html`.

### 8. Internal Linking & Media
- Use clear internal links (real `<a href>`), sensible anchor text, and `alt` text for images. Avoid blocking required JS/CSS for rendering.

## Best Practices

### 1. Titles & Descriptions
- One unique `<title>` per page, avoid boilerplate and keyword stuffing. Make the main visual title consistent.
- Provide a concise meta description that truly summarizes the page.

### 2. Canonical, Sitemap & Indexing
- Add a self-referential `<link rel="canonical">` on canonical pages.
- Keep sitemap URLs canonical, update on deploy.
- Keep `robots.txt` at root, allow essential resources. Don’t accidentally disallow JS/CSS needed for rendering.

### 3. Structured Data
- Use JSON-LD that matches on-page content.
- Don’t add markup for content that isn’t present.

### 4. Social Preview
- Keep social previews (e.g. OG/Twitter tags) consistent with the SEO title and description.

---

## Code Review

Only fix SEO-related code, do not change anything else.

### 1. Indexability & Rendering
- Scan the meaningful content from the initial HTML, ensuring avoid any blocked resources.

### 2. Titles & Descriptions
- Ensure each page has exactly one unique <title> tag. Confirm meta description is present.

### 3. Canonical & Robots
- Self-canonical on canonical pages. `robots.txt` doesn’t block critical pages/resources.

### 4. Sitemap
- XML sitemap exists, lists canonical URLs, referenced in `robots.txt`.

### 5. Structured Data
- JSON-LD present where applicable and consistent with visible content. Validate types and required properties.

### 6. Headings & Content
- Logical H1/H2 hierarchy. Main topic clear, important copy not hidden behind tabs/JS.

### 7. Internal Links & Media
- Crawlable `<a href>` links. Descriptive anchor text that images have meaningful `alt`.

### 8. Page 404
- Functional `/404.html`.

---

## Checklist
Respond with a summary and a checklist indicating which tasks above are completed.

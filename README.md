# Richard Basile — Site README

## Local Preview

### Prerequisites
Make sure you have Ruby and Bundler installed.

If you don't have a `Gemfile` in your repo root, create one with:

```ruby
source "https://rubygems.org"

gem "github-pages", group: :jekyll_plugins
```

Then install dependencies once:

```bash
bundle install
```

This will create a `Gemfile.lock` — commit both files to your repo.

### Start the Local Server

```bash
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000) in your browser.

> **Note:** Any changes you save to `.md` files will hot-reload automatically. However, if you change `_config.yml`, you must stop the server (`Ctrl+C`) and restart it for changes to take effect.

---

## Writing a New Blog Post

1. Create a new file in the `_posts/` directory named using this format:

```
_posts/YYYY-MM-DD-your-post-title.md
```

For example: `_posts/2025-03-07-my-first-run.md`

2. Add front matter at the top of the file:

```yaml
---
layout: default
title: "Your Post Title"
date: 2025-03-07
---
```

3. Write your content below the front matter in Markdown.

---

## Updating the Links Page

Edit `links.md` in the repo root. Each link follows this format:

```markdown
- <i class="fab fa-icon-name"></i> [Label](https://url)
```

Icon names come from [Font Awesome](https://fontawesome.com/icons).

---

## Updating Site Settings

Edit `_config.yml` for:
- **Site title or description**
- **Header navigation pages** (`header_pages`)
- **Author info and social links**

Remember to restart your local server after any `_config.yml` change.

---

## Publishing Changes

```bash
git add .
git commit -m "Your commit message"
git push
```

GitHub Pages will automatically rebuild and publish the site within a minute or two. Check the **Actions** tab in your GitHub repo to monitor the build status.
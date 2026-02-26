# jctrent.com

Author website for J.C. Trent, built with [Jekyll](https://jekyllrb.com/) and hosted on [GitHub Pages](https://pages.github.com/).

## Local development

```bash
# Install Jekyll (one-time)
gem install bundler jekyll

# Serve locally
bundle exec jekyll serve
```

Site will be available at `http://localhost:4000`.

## Structure

```
├── _config.yml          # Site configuration
├── _layouts/
│   └── default.html     # Shared page layout
├── _includes/
│   ├── nav.html         # Navigation bar
│   └── footer.html      # Footer
├── assets/
│   ├── css/style.css    # Stylesheet
│   └── img/             # Images (covers, etc.)
├── index.html           # Home page
├── books.html           # Books page
├── about.html           # About page
└── pipeline.html        # Build pipeline writeup
```

## Adding a page

Create a new `.html` or `.md` file in the root with front matter:

```yaml
---
layout: default
title: Page Title
---
```

Add a nav link in `_includes/nav.html`.

## Custom domain

1. Add a `CNAME` file containing your domain (e.g. `jctrent.com`)
2. Point your DNS: CNAME record → `yourusername.github.io`
3. Enable HTTPS in repo Settings → Pages

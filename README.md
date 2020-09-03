# Setup Instructions

1. Clone repository to your computer.
2. Using terminal, navigate to the `cheat-codes-docs` directory with `cd`.
3. In the directory type `bundle exec jekyll serve --baseurl ''`.
4. Visit [http://127.0.0.1:4000](http://127.0.0.1:4000) in your browser.

## Adding Pages

Just add a new `your-page-name.md` file in the `_pages` directory. At the top of the file, add this "frontmatter":

```
---
layout: page
title: "your page name"
permalink: /your-page-name
---
```

This is where you configure the page title and permalink. They can be anything you want.

## Navigation

Configure main navigation with `_data/nav.yml`.

## CSS

To work with the CSS: `cd assets/stylesheets` and run `sass --watch style.sass:style.css`.

# ventralvex.github.io

My personal website, built with Jekyll and the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme, hosted on GitHub Pages.

## Editing content

- **Home page text**: edit [index.md](index.md).
- **Name, email, LinkedIn, GitHub, bio**: edit the `author` (and `footer`) section in [_config.yml](_config.yml).
- **Profile photo**: replace [assets/images/profile.jpg](assets/images/profile.jpg) with your own photo (keep the same filename, or update the `avatar` path in `_config.yml`).

## Adding a new page (e.g. a CV)

1. Add a new Markdown file to the `_pages/` folder, e.g. `_pages/cv.md`, with front matter like:

   ```yaml
   ---
   layout: single
   title: "CV"
   permalink: /cv/
   ---
   ```

2. Add the page to the site navigation by adding an entry to [_data/navigation.yml](_data/navigation.yml):

   ```yaml
   main:
     - title: "Home"
       url: /
     - title: "CV"
       url: /cv/
   ```

## Local preview

```
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000`.

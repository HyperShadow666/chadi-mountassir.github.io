# chadi-mountassir.github.io

Personal site and blog, built with [Hugo](https://gohugo.io) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme. Pushing to `main` builds and deploys it through `.github/workflows/hugo.yml`.

## Setup

```bash
git submodule update --init --recursive   # fetch the theme
hugo server -D                            # preview at http://localhost:1313 (includes drafts)
```

## Writing a post

```bash
hugo new posts/my-post-title.md
```

Edit `content/posts/my-post-title.md`, set `draft: false` when it's ready, then commit and push.

- Images: put them next to the post as a page bundle (`content/posts/my-post/index.md` + `figure.png`) or in `static/`.
- Math: add `math: true` to the front matter, then use `\( ... \)` inline and `$$ ... $$` for display equations.
- Tags: `tags: ["llm", "mlops"]` in the front matter.

## Other content

- `content/about.md`: the About / résumé page
- `static/cv_chadi_moutassir.pdf`: the CV linked from the menu
- `hugo.toml`: site title, intro text, menu and social links

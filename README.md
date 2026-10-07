# Nate's Place

Fresh Hugo site for https://jimmytortilla.github.io/natesplace/

Theme: [hugo-bearblog](https://github.com/janraasch/hugo-bearblog), the Hugo port of Herman's Bear Blog. No analytics. No JavaScript except a Vimeo iframe when a post includes one.

The theme is already in `themes/hugo-bearblog`.

## Replace the old repo

On GitHub, delete `jimmytortilla/natesplace`, then create an empty repo with the same name. Do not add a README.

```bash
cd natesplace-bear
git init -b main
git add .
git commit -m "Fresh Bear Blog site"
git remote add origin git@github.com:jimmytortilla/natesplace.git
git push -u origin main
```

Then: repo Settings → Pages → Build and deployment → Source: GitHub Actions.

The site will be at https://jimmytortilla.github.io/natesplace/

## Preview in Termux

```bash
pkg install hugo git
hugo server -D --bind 127.0.0.1 --baseURL http://127.0.0.1:1313/natesplace/ --noBuildLock
```

Open http://127.0.0.1:1313/natesplace/

## New post with a photo and a video

```bash
hugo new blog/makohood/index.md
```

Put `yard.jpg` in `content/blog/makohood/` next to `index.md`.

```markdown
+++
title = "Makohood"
date = 2026-10-07
draft = false
+++

A short note.

![Back yard](yard.jpg)

{{< vimeo id="1233614089" title="Makohood" >}}
```

The Vimeo id is the number in `player.vimeo.com/video/1233614089`. Commit the folder and push. Actions publishes it.

A later custom domain (`.life` or similar) is a one-line `baseURL` change plus a `static/CNAME` file. Not needed yet.

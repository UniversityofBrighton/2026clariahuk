# CLARIN & DARIAH UK Annual Event — website

A [Jekyll](https://jekyllrb.com) site, ready for **GitHub Pages** (`username.github.io`).

## Where the text lives (edit these — no HTML needed)

| To change… | Edit this file |
|---|---|
| Home intro & hero copy | `index.md` |
| Programme sessions | `_data/schedule.yml` |
| Speakers | `_data/speakers.yml` |
| Venue directions | `_data/travel.yml` + intro in `venue.md` |
| About text, themes, audiences | `about.md` + `_data/about.yml` |
| Registration | `register.md` |
| Event date / venue / hosts / nav | `_config.yml` |
| Colours, fonts, layout | `assets/style.css`, `_layouts/default.html` |

The `.yml` files are simple lists — copy an existing block to add another
session or speaker. To add a speaker photo, drop the image in
`assets/speakers/` and set `photo: /assets/speakers/name.jpg` in
`_data/speakers.yml`.

## Preview locally
```
cd site
bundle install
bundle exec jekyll serve
```
Open http://localhost:4000

## Publish on GitHub Pages
1. Create a repo and push the **contents of this `site/` folder** to it.
2. Repo → **Settings → Pages** → Source: *Deploy from a branch* → `main` / root.
3. **Project site** (`username.github.io/REPO`): set `baseurl: "/REPO"` in
   `_config.yml`. **User/org site** (`username.github.io`): leave `baseurl: ""`.

Your site builds automatically at the URL shown in Settings → Pages.

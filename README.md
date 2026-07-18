# CLARIN & DARIAH UK Annual Event — website

A [Jekyll](https://jekyllrb.com) site, ready for **GitHub Pages** (`username.github.io`).

## Where the text lives (edit these — no HTML needed)

| To change… | Edit this file |
|---|---|
| Home intro & hero copy | `index.html` |
| Programme sessions | `_data/schedule.yml` |
| Speakers | `_data/speakers.yml` |
| Venue directions | `_data/travel.yml` + intro in `venue.html` |
| About text, themes, audiences | `about.html` + `_data/about.yml` |
| Registration | `register.html` |
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

## Publish on GitHub Pages (GitHub Actions — recommended)

This repo includes `.github/workflows/jekyll.yml` (GitHub's official Jekyll
workflow), so deployment is automatic.

1. Push the **contents of this `site/` folder to the repo root** (so
   `_config.yml`, `Gemfile` and `.github/` sit at the top level).
2. Repo → **Settings → Pages** → Source: **GitHub Actions**.
3. Push to `main`. The workflow builds and deploys; the live URL appears in
   the Actions run and in Settings → Pages.

Leave `baseurl: ""` in `_config.yml` — the workflow injects the correct base
path automatically (`--baseurl`), and all links use `relative_url`, so they
resolve on both user sites and project sites with no edits.

> Building from the repo root is required — the workflow runs `jekyll build`
> there. If you'd rather keep the files inside a `site/` subfolder, add
> `defaults: { run: { working-directory: site } }` to the build job, set
> `working-directory: site` on the Setup Ruby step, and change the artifact
> path to `site/_site`.

## Publish without Actions (deploy from a branch)
Alternatively, Settings → Pages → Source: *Deploy from a branch* → `main` /
root. In that mode, set `baseurl: "/REPO"` for a project site.

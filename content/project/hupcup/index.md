---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Hupcup"
summary: "Sync your github forks without Git or Node."
authors: [admin]
tags: ["tools"]
categories: []
date: 2021-02-28T17:59:42+08:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/ritou11/hub-cup"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
Sync your github forks without Git or Node. This is the Go version of [hub-sync](https://github.com/b1f6c1c4/hub-sync). You could use binary files rather than heavy envirnoments.

## Download Binary

Prebuilt binaries available at https://github.com/ritou11/hub-cup/releases

## TL;DR

```sh
# Generate a token **with public_repo scope** at https://github.com/settings/tokens
echo the-token > ~/.hub-cup
# Update your webpack fork default branch to the latest of upstream:
hub-cup webpack
# Update your material-ui fork default branch to the latest of upstream:
hub-cup material-ui
# Update your material-ui fork master branch to the latest of upstream:
hub-cup material-ui/master
# Update your antediluvian io.js fork to the latest nodejs:
hub-cup io.js # name doesn't need to match exactly
hub-cup io.js nodejs/node # but you MUST specify the repo if you want to sync to the upstream of upstream
```

## Usage

```
NAME:
   hub-cup - Make your github forks catch up with origins

USAGE:
   hub-cup <what> [<from>]

VERSION:
   0.1.0

AUTHOR:
   Nogeek <ritou11@gmail.com>

GLOBAL OPTIONS:
   --token value, -t value  Github token, see https://github.com/settings/tokens
   --token-file path        path to your Github token file (default: "~/.hub-cup")
   --force, -f              As if {git push --force}
   --dry-run, -n            Don't actually update
   --debug                  print debug messages
   --help, -h               print the help
   --version, -v            print the version
```

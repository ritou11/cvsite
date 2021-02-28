---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Dictconv"
summary: "A Mac dictionary converter based on Node.js. You could convert some additional dictionaries and install them on your Mac dictionary app."
authors: []
tags: ["tools"]
categories: []
date: 2021-02-28T18:06:17+08:00

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

url_code: ""
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

## TL;DR

`dictconv convert <stardict_xxxxx.tar.bz2> -i -v`
Building would take some time, please be patient.

## Background
A Node.js version of [DictUnifier](https://github.com/jjgod/mac-dictionary-kit). The original repo is no longer maintained, while I really want a converter for the Stardicts.

Require Node.js >= 12 to support ES module.

## Installation

`yarn global add @ritou11/dictconv` or `npm i -g @ritou11/dictconv`

You'll also need `gunzip`, `tar`,`cp`,`mkdir` in your system path. They should be installed with MacOSX already.

## Usage
```
dictconv [command]

Commands:
  dictconv raw <stardict> <destPath>        Convert the startdict to xml
                                            dictionary.
  dictconv build <rawPath> [<destPath>]     Build the Mac dictionary from raw
                                            data
  dictconv convert <stardict> [<destPath>]  Convert the startdict to Mac
                                            dictionary.

Options:
  --version   Show version number                                      [boolean]
  -h, --help  Show help                                                [boolean]
```
```
dictconv raw <stardict> <destPath>

Convert the startdict to xml dictionary.

Positionals:
  stardict  <stardict> The path to the stardict file.        [string] [required]
  destPath  <destPath> The destination path.                 [string] [required]
```
```
dictconv build <rawPath> [<destPath>]

Build the Mac dictionary from raw data

Positionals:
  rawPath  <rawPath> The path to the raw data files.         [string] [required]

Options:
  --version      Show version number                                   [boolean]
  --name, -n     The name of dictionary                                 [string]
  --install, -i  Install the converted dictionary to the system
                                                      [boolean] [default: false]
```
```
dictconv convert <stardict> [<destPath>]

Convert the startdict to Mac dictionary.

Positionals:
  stardict  <stardict> The path to the stardict file.        [string] [required]
  destPath  <destPath> The destination path.                            [string]

Options:
  --version      Show version number                                   [boolean]
  --name, -n     The name of dictionary                                 [string]
  --install, -i  Install the converted dictionary to the system
                                                      [boolean] [default: false]
```

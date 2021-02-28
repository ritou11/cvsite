---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Xuetangxd"
summary: "A downloader for next.xuetangx.com. NPM package is provided."
authors: [admin]
tags: ["tools"]
categories: []
date: 2021-02-28T17:53:41+08:00

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

url_code: "https://github.com/ritou11/xuetangxd"
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
This project is a downloader for next.xuetangx.com.

## Usage

1. ```yarn global add @ritou11/xuetangxd``` or ```npm i -g @ritou11/xuetangxd```
2. Add a config file ```~/.xuetangxd``` in the following format:
   ```
   {
       "username": "<Username>",
       ["rsaPassword": "<Password hashed by RSA>",]
       ["password": "<Clear text password>",]
   }
   ```
* rsaPassword could be got by providing the clear text password and `xuetangxd dryrun`.
3. Command format:
```
xuetangxd [command]

Commands:
  xuetangxd dryrun                    show the info & donnot execute
  xuetangxd prepare [<cid>] [<sign>]  prepare the course cache file
  xuetangxd fetch                     fetch the course videos
  xuetangxd down [<cid>] [<sign>]     get the course video links

Options:
  --version           Show version number                              [boolean]
  -c, --config-file   Json file that contains username, md5_password and other
                      infomation.             [string] [default: "~/.xuetangxd"]
  -u, --username      Username of your account.                         [string]
  -p, --password      Plaintext password of your account.               [string]
  -m, --rsa-password  RSA password of your account.                     [string]
  -f, --cache-file    Use specified cache file to start                 [string]
  -o, --output-file   output cache file to the path                     [string]
  -q, --quality       High quality or not                              [boolean]
  --help              Show help                                        [boolean]
```
4. `<cid>` and `<sign>` is from the link of the course, which follows `https://next.xuetangx.com/course/<sign>/<cid>`.

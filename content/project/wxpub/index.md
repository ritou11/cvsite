---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "WeChat official account visualization"
summary: "[CHINESE ONLY] Analyze the wechat official accounts."
authors: [admin]
tags: []
categories: []
date: 2021-02-28T17:12:16+08:00

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

url_code: "https://github.com/ritou11/wxPubVis"
url_pdf: ""
url_slides: ""
url_video: "https://www.bilibili.com/video/BV1wX4y1V7Xm"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
This project includes the frontend part and backend part. Though the frontend is still [deployed](https://wxpub.nogeek.top), the backend is down because of the bill. Even though, I hope the [source code](https://github.com/ritou11/wxPubVis) could be helpful.

Basically, in the backend, we crawler the publications of an official account by proxy. Then, all the information is stored in MongoDB. We also have a service following GraphQL. The frontend is deployed by Netlify and get necessary data by GraphQL from the backend. The visualization part is based on D3.js.

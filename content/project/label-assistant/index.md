---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Scene-Text Label Assistant"
summary: "Cross-Platform Automatic Scene-Text Label Assistant"
authors: ["admin"]
tags: ["Computer Vision"]
categories: []
date: 2019-11-14T22:23:56+08:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Smart"
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/Joinn99/KirinLabelAssistant"
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

**Scene-Text Label Assistant** is a **Cross-Platform** desktop computer program with user friendly GUI interface, which helps to create training set for **Scene Text Detection**. Users can use the program to label their own images efficiently with the help of the automatic label function, which utilized [EAST neural network](https://arxiv.org/abs/1704.03155v2) to generate labels automatically. Users only need to correct few model's wrong label results.

It is programmed in C++ with [Qt](https://www.qt.io/) framework. The EAST model applied in the program by using [OpenCV](https://opencv.org/) Library.

Here are some of the examples using the software:
![scree-shot-1](screen1.jpg)

![scree-shot-2](screen2.jpg)
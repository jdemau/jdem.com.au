---
title: Hi,
layout: splash
permalink: /
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/banner.jpg
excerpt: >
  We're Emma & Jaidev. <br /> A couple from Brisbane, Australia.
feature_row_em:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row_jd:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
  ---

{% include feature_row id="feature_row_em" type="left" %}

{% include feature_row id="feature_row_jd" type="right" %}
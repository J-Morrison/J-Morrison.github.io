---
permalink: /
hidden: true
layout: splash
author_profile: false
header:
  overlay_image: "/assets/images/cover.jpg"
  overlay_filter: 0.15
  actions:
excerpt: "Aspiring controls engineer interested in bridging the gap between control theory and machine learning"
intro: 
  - excerpt: "Hey! Welcome to my personal website. Feel free to poke aroud to learn a little bit more about me, my interests, my background, and some of the things I've been up to."
feature_row:
  - image_path: /assets/images/circle-cropped.png
    title: "About"
    excerpt: "Discover a little bit about who I am and what interests me."
    url: /about/
    btn_label: "Learn More"
    btn_class: "btn--inverse"
  - image_path: /assets/images/circle-cropped.png
    title: "Projects"
    excerpt: "Take a look at some of the projects I've completed"
    url: /projects/
    btn_label: "Explore"
    btn_class: "btn--inverse"
  - image_path: /assets/images/circle-cropped.png
    title: "Resume"
    excerpt: "View an up to date version of my resume in pdf format."
    url: /Resume/
    btn_label: "Download"
    btn_class: "btn--inverse"
---
{% include feature_row id="intro" type="center" %}
{% include feature_row %}

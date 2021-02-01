---
permalink: /
hidden: true
layout: splash
author_profile: false
header:
  overlay_image: "/assets/images/cover.png"
  overlay_filter: 0.2
  actions:
#    - label: "Connect"
#      url: "https://www.linkedin.com/in/morrisonjacob"
    - label: "Get In Touch"
      url: "mailto:jacob-morrison@outlook.com"
excerpt: "Software engineer interested in machine learning and its applications"
intro: 
  - excerpt: "Hey, welcome to my website! I'm Jacob and I am currently based in Vancouver, Canada, where I am working as a Software Engineer at MDA. Feel free to poke around to learn a little more about me."
feature_row:
  - image_path: /assets/images/about.png
    title: "About"
    excerpt: "Discover a little bit about who I am and what interests me."
    url: /about/
    btn_label: "Learn More"
    btn_class: "btn--inverse"
  - image_path: /assets/images/proj.png
    title: "Projects"
    excerpt: "Take a look at some of the projects I've worked on."
    url: /projects/
    btn_label: "Explore"
    btn_class: "btn--inverse"
  - image_path: /assets/images/resume.png
    title: "Resume"
    excerpt: "Scan through the current iteration of my resume in pdf format."
    url: /resume/JacobMorrison_Resume.pdf
    btn_label: "View"
    btn_class: "btn--inverse"
---
{% include feature_row id="intro" type="center" %}
{% include feature_row %}

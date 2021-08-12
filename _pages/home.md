---
title: "Hello!"
layout: splash
permalink: /
hidden: true
author_profile: true
header:
  overlay_color: "#5e616c"
  overlay_filter: linear-gradient(rgba(255, 0, 0, 0.5), rgba(0, 255, 255, 0.5))
  overlay_image: /assets/images/mm-home-page-feature.jpg
  actions:
    - label: "<i class='fas fa-info-circle'></i> About"
      url: "/docs/quick-start-guide/"
excerpt: >
  Welcome to SeungU Lyu's website! <br />
feature_row:
  - image_path: /assets/images/mm-customizable-feature.png
    alt: "customizable"
    title: "Current Projects"
    excerpt: "On-going projects"
    url: "/docs/configuration/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/mm-responsive-feature.png
    alt: "fully responsive"
    title: "Old Projects"
    excerpt: "Old projects done before"
    url: "/docs/layouts/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/mm-free-feature.png
    alt: "100% free"
    title: "Blog"
    excerpt: "My daily thoughts"
    url: "/docs/license/"
    btn_class: "btn--primary"
    btn_label: "Learn more"  
gallery3:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Blog"
  - image_path: /assets/images/unsplash-gallery-image-4-th.jpg
    alt: "placeholder image 4"    
---

{% include feature_row %}

{% include gallery id="gallery3" %}
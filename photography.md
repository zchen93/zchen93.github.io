---
layout: splash
title: "Photography"
permalink: /photography/
gallery:
  - image_path: /assets/images/gallery/IMG_5537.jpg
    title: "Approaching Maui"
    alt: "Approaching Maui"
  - image_path: /assets/images/gallery/IMG_7178.jpg
    title: "Golden hour - Aspen, CO"
  - image_path: /assets/images/gallery/IMG_4789.jpg
    title: "Lake in the morning - Wind River Reservation, Wyoming"
  - image_path: /assets/images/gallery/IMG_6107.jpg
    title: "Dancing girl by the sea - The Island of Hawaii"
  - image_path: /assets/images/gallery/IMG_6062.jpg
    title: "Observatory - Mauna Kea, The Island of Hawaii"
  - image_path: /assets/images/gallery/IMG_6018.jpg
    title: "Tranquility - The Island of Hawaii"
  - image_path: /assets/images/gallery/IMG_6013.jpg
    title: "Trail and volcano - The Island of Hawaii"
  - image_path: /assets/images/gallery/IMG_5817.jpg
    title: "Trail leads into the cloud - Haleakala NP, Maui"
  - image_path: /assets/images/gallery/IMG_1030.jpg
    title: "Golden Gate Bridge - San Francisco, CA"
---

A quiet observer's journey through the world's untamed places.

<div class="photography-gallery">
  {% for img in page.gallery %}
    <figure>
      <a href="{{ img.image_path }}" class="image-popup" title="{{ img.title }}">
        <img src="{{ img.image_path }}" alt="{{ img.title }}">
      </a>
      <figcaption>
        <strong>{{ img.title }}</strong><br>
        {{ img.caption }}
      </figcaption>
    </figure>
  {% endfor %}
</div>
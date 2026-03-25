---
layout: splash
title: "Photography"
permalink: /photography/
gallery:
  - image_path: /assets/images/gallery/IMG_5537.JPG
    title: "Approaching Maui"
    alt: "Approaching Maui"
  - image_path: /assets/images/gallery/IMG_7178.JPG
    title: "Golden hour - Aspen, CO"
  - image_path: /assets/images/gallery/IMG_4789.JPG
    title: "Lake in the morning - Wind River Reservation, Wyoming"
  - image_path: /assets/images/gallery/IMG_6107.JPG
    title: "Dancing girl by the sea - The Island of Hawaii"
  - image_path: /assets/images/gallery/IMG_6062.JPG
    title: "Observatory - Mauna Kea, The Island of Hawaii"
  - image_path: /assets/images/gallery/IMG_6018.JPG
    title: "Tranquility - The Island of Hawaii"
  - image_path: /assets/images/gallery/IMG_6013.JPG
    title: "Trail and volcano - The Island of Hawaii"
  - image_path: /assets/images/gallery/IMG_5817.JPG
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
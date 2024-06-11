---
layout: post
title: Help choose a logo
date: 2024-06-11 10:00:00
description: BIG Culture is still using a default icon, let's get a new one
tags:
categories:
featured: true
giscus_comments: true
thumbnail: assets/img/speakers/herrema_ron.png
images:
  slider: true
---

# How to Add a Logo for Discussion

Add the logo to the directory: assets/img/blog/logos/  
Add the below code to the Logos section of this page, replacing LOGO_NAME.EXT with your logo (e.g., logo1.png):

```liquid
'{% include figure.liquid loading="eager" path="assets/img/9.jpg" class="img-fluid rounded z-depth-1" %} '
```

# Logos
{% include figure.liquid loading="eager" path="assets/img/blog/logos/logo1.png" class="img-fluid rounded z-depth-1" %} {% include figure.liquid path="assets/img/blog/logos/logo2.png" class="img-fluid rounded z-depth-1" zoomable=true %} {% include figure.liquid path="assets/img/blog/logos/logo3.png" class="img-fluid rounded z-depth-1" zoomable=true %} {% include figure.liquid path="assets/img/blog/logos/logo4.png" class="img-fluid rounded z-depth-1" zoomable=true %}
---
title:  "Age Estimation from Rhytides"
permalink: "/posts/age-estimation-from-rhytides"
categories: ["data", "computer-vision"]
header:
  teaser: /assets/images/projects/age-estimation-from-rhytides.jpg
excerpt: >
  A computer vision project with the goal of detecting and quantifying facial wrinkles (rhytides) for age estimation.
---

In spring 2021 another graduate student and I did a project for our computer vision class which involved trying to detect and quantify facial wrinkles (rhytides) in face images for age estimation &mdash; an open computer vision problem.

Our approach involved using face detection to create bounding polygons on various regions of the face in the [UTKFace](https://susanqq.github.io/UTKFace/) dataset, then doing edge detection within each polygon to quantify wrinkles in the area.

Ultimately, we found that variations in lighting and facial expressions cause enough noise to make this method unreliable for estimating age. However, the project was an interesting one, and we created [a smaller but cleaner subset of UTKFace with only higher-quality images](https://github.com/tomreitz/cs766-computer-vision-project/tree/main/data/UTKFace-cleaned.zip) which may be useful to other researchers.

<center>
<a class="btn btn--info btn--primary" href="https://tomreitz.github.io/cs766-computer-vision-project/" target="_blank">Project page</a>
<a class="btn btn--info btn--primary" href="https://github.com/tomreitz/cs766-computer-vision-project/tree/main/code" target="_blank">Code</a>
<a class="btn btn--info btn--primary" href="https://docs.google.com/presentation/d/1aJU_h0YStWdd_LNF0Sg-z33jkzOfN0_mpU_Pu-ZvVHo/edit?usp=sharing" target="_blank">Slides</a>
<br />
</center>


Below is a video presentation about the project:

{% include video id="TrRghR6Su7I" provider="youtube" %}

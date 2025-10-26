---
layout: page
title: MolVisWeb
description: A web-based, accessible, 3D molecular visualization software platform to increase access to STEM education. 
img: assets/img/molvisweb/thumbnail.jpg
importance: 1
category: work
related_publications: false
---

In my senior year, I completed an undergraduate thesis in the Computer Science and Chemistry departments. I was advised by <a href="https://www.wellesley.edu/people/mala-radhakrishnan">Dr. Mala Radhakrishnan</a> in the Chemistry Department and <a href="https://www.wellesley.edu/people/scott-anderson">Dr. Scott Anderson</a> in the Computer Science Department, with additional mentorship from members of my thesis committee in human-computer interaction and software development. 

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include video.liquid path="assets/video/molvisweb_demo.mp4" title="MolVisWeb software demo" class="img-fluid autoplay rounded z-depth-1" %}
    <div class="caption">
        Above, I provide a quick video demonstration of how MolVisWeb functions.
    </div>
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/molvisweb/thesis_cover_page.png" title="Thesis Cover Page" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

Chemical bonding is a critical part of learning introductory chemistry, but is often a difficult concept for students to grasp. The <a href="https://pubs.acs.org/doi/full/10.1021/acs.jchemed.4c00036">EMMAs</a> (Exploring Molecular Modeling Activities) are a series of educational activities designed by <i>Kotsalidis et al.</i> to teach high school chemistry students about noncovalent bonding through case studies and exploratory exercises using the 3D molecular visualization tool <a href="https://www.ks.uiuc.edu/Research/vmd/">VMD</a> (Visual Molecular Dynamics). However, VMS isn't available on Chromebookes, the most commonly-used PCs by high school students, and it also requires installation. Thus, the motivation behind my thesis is to build and evaluate a web-based molecular visualization interface that implements the EMMAs, which will make these activities accessible to more students.

Check out the <a href="https://github.com/maya-mau/molvisweb_thesis_version">gihub repository</a> to see my code, and <a href="https://maya-mau.github.io/molvisweb_thesis_version/">MolVisWeb</a> itself to experiment with the platform and hopefully learn something new about drug-protein interactions. MolVisWeb was mainly coded in Javascript using the package <a href="https://threejs.org/">Three.js</a> to render 3D visuals. 


<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/molvisweb/thesis_defense.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="caption col-sm-4">
        A photo from my successful thesis defense in May 2025. From left to right: <a href="https://cs.wellesley.edu/~cbassem/">Dr. Christine Bassem</a>, <a href="https://www.wellesley.edu/people/vinitha-gadiraju">Dr. Vinitha Gadiraju</a>, <a href="https://www.wellesley.edu/people/scott-anderson">Dr. Scott Anderson</a>, myself, <a href="https://www.wellesley.edu/people/mala-radhakrishnan">Dr. Mala Radhakrishnan</a>, and <a href="https://www.wellesley.edu/people/ann-velenchik">Dr. Ann Velenchik</a>. 
    </div>
</div>

<br>
Lastly, some fun bloopers from my many hours of late-night coding and debugging. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/molvisweb/blooper_1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/molvisweb/blooper_2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/molvisweb/blooper_3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

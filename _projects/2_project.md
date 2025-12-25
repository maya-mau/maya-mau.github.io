---
layout: page
title: Hapestry
description: A neural network genotyper to predict the existence of structural variants in DNA.
img: assets/img/hapestry/broad_building.jpg
importance: 2
category: work
related publications: false
---

Last summer, I had the opportunity to explore bioinformatics and machine learning at the <a href="https://www.broadinstitute.org/">Broad Institute of MIT and Harvard</a>. I was advised by Dr. Fabio Cunial and Dr. Ryan Lorig-Roach on the Long Reads team, a part of the Data Sciences Platform (DSP). 

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/hapestry/broad_group.jpeg" title="Group photo in front of the Broad Institute building in Cambridge, MA" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="caption col-sm-4">
        A group photo of all the Long Reads summer research assistants at the end of the program in August 2025. 
    </div>
</div>

During my three-month internship, I worked on Hapestry, a neural network genotyper that reconstructs structural variants from DNA sequencing data. Structural variants (SVs) are important because they can help predict disease. DNA sequencing technology has evolved throughout the years, from laborious first-generation sequencing techniques to modern sequencing techniques that enabled the completion of the Human Genome Project [1]. Today, many different sequencing techniques exist, each with various strengths and weaknesses that contribute to cost and read accuracy. Long-read sequencing (by companies such as PacBio and Oxford Nanopore) involves analyzing long fragments of DNA that are thousands of base pairs long. Short-read sequencing (by companies such as Illumina), by contrast, analyze shorted fragments of DNA that range from 30-500 base pairs long. Long-read sequencing data is more accurate but more expensive than short-read sequencing data [2].

Another factor that contributes to read accuracy and cost is depth of coverage, or how many times each base is read. Short-read sequencing is usually high coverage (e.g. 30x), while long-read sequencing is usually low coverage (e.g. 5x). Theoretically, high coverage long-read sequencing data would provide the most accurate variant calls, although such technology is impractically expensive. By contrast, low coverage long-read data and high coverage short-read are less expensive but individually less accurate. 

We hypothesized that Hapestry's performance would improve when given features extracted from both high coverage short-read and low coverage long-read sequencing data. This theory proved true: combining features from 4x long-read and 32x short-read data improved genotyping performance, though our findings revealed unexpected differences across variant-stratified groups that warranted further investigation. To evaluate Hapestry, I stratified performance data by variables such as base pair length and variant type to pinpoint the model's strengths and weaknesses, using typical neural network metrics like ROC and AUC.  

My summer at the Broad opened me up to the world of computational biology and applied machine learning, topics that I found fascinating and am eager to pursue further. At the end of the program, I presented on my research at the monthly DSP meeting, and was able to hear about the research my fellow summer research assistants were conducting. Through my research, I learned how to use the Integrative Genomics Viewer, or IGV, a data visualization tool that can visualization different types of genomic data. I also gained experience in data stratification and neural networks. Ultimately, my most important takeaway was that I could pick up new skills quickly with mentorship and guidance. When I initially applied to this position, I was nervous--I had no previous formal training in genomics, and the last time I took biology was in the 9th grade. However, my mentors and other Broad scientists were extremely welcoming and willing to answer questions, which helped me onboard quickly and dive into the research.

My experience straddling industry and academia at the Broad also motivated me to pursue graduate education. Although I really enjoyed the coding and development aspect of my work, I also loved the environment of constant learning around me. The Broad hosts many weekly seminars and talks, inviting scientists from around the world to share their work. I attended as many talks as I could--I understood very little of the majority, but being exposed to the world of academia and research encouraged me to explore options for continued education. 

<br>
Lastly, I really enjoyed spending the summer in Cambridge and Boston. Here are some photos I took that summer with my mom's old digital camera. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/hapestry/charles_1.JPG" title="The Charles River during sunset." class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/hapestry/esplanade_1.JPG" title="A person sitting in a tree framed by the sunset along the esplanade." class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/hapestry/esplanade_2.JPG" title="People socializing on a dock at dusk along the Charles River." class="img-fluid rounded z-depth-1" %}
    </div>
</div>

[1] <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC4727787/">https://pmc.ncbi.nlm.nih.gov/articles/PMC4727787/</a>

[2] <a href="https://www.cd-genomics.com/longseq/resource-long-read-vs-short-read-sequencing.html">https://www.cd-genomics.com/longseq/resource-long-read-vs-short-read-sequencing.html</a>

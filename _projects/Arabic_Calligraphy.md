---
layout: page
title: Arabic Calligraphy
description: Arabic Calligraphy Style Detection and Character Recognition
img: assets/img/calligraphy.png
importance: 4
category: work
selected: true

authors:
  - name: AJEGHRIR Mustapha
    url: "/"
    affiliations:
      name: Student, CentraleSupelec


---


The github repository : 
<div style= "text-align: center;">
    <div class="github-card" data-github="Mustapha-AJEGHRIR"  data-repo="arabic_calligraphy" data-height="" data-theme=""></div>
    <script src="//cdn.jsdelivr.net/github-cards/latest/widget.js"></script>
</div>


In this project we were a team of 3 students : 
- Mustapha Ajeghrir
- Nouamane Tazi
- Asmae Khald


This project is separated in two parts, the first one is an introduction to the project and it aims to recognise the style of the Arabic calligraphy. The second part and the main part aims to recognize the characters and words from the calligraphy.

## `ACSR` (Arabic Calligraphy Style Recognition):
Our implementation is highly inspired from [ArbMl](https://github.com/ARBML/ARBML)'s work and the data (synthetic and real) from [Mahmoud Aslan](https://mhmoodlan.github.io/blog/arabic-font-classification#4-data)'s collection. The main problem in `ACSR` (Arabic Calligraphy Style Recognition) is the scarcity of data. Hopefully, it is possible to generate data using digital fonts to help the training, the model is then tested on the real data reaching a score of 97% in accuracy. The used architecture is a simple CNN network (more on that in the full report in the end of this article). We have also managed to perform some saliency maps as shown in the figure below. 

{% include figure.html path="assets/img/atabic_saliency_maps.jpg" class="img-fluid rounded z-depth-1" %}

#### Demo 
A demo could be accessed is the following HuggingFace spaces link : [https://huggingface.co/spaces/mustapha/ACSR](https://huggingface.co/spaces/mustapha/ACSR)

## `OCR` (optical character recognition):
The main inspiration of this part is [TrOCR](https://www.researchgate.net/publication/354751878_TrOCR_Transformer-based_Optical_Character_Recognition_with_Pre-trained_Models) paper. It uses a `Vision-Encoder-Decoder` model. For the encoder we used the ViT model, which applies a pure transformer directly to sequences of image patches to classify the full image. Its embeddings are then passed to the decoder. This decoder uses the weights of AraBERT. The figure below shows the architecture of the model.

{% include figure.html path="assets/img/model_trocr.png" class="img-fluid rounded z-depth-1" %}

## For A detailed description :
Below is our report for this project, please feel free to read it and email me if necessary.
<iframe src="/assets/pdf/Rapport_arabic_calligraphy.pdf" style="width:100%; height:500px;" frameborder="0"></iframe>
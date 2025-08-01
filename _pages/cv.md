---
layout: archive
#title: "Curriculum Vitae | Ishaq Muhammad"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 1em;">
  <h1 style="margin: 0;">Curriculum Vitae | Ishaq Muhammad</h1>
  <a href="{{ '/files/cv.pdf' | relative_url }}" download
     style="text-decoration: none; padding: 0.4em 0.8em; background-color: #007acc; color: white; border-radius: 4px;">
    CV.pdf
  </a>
</div>

Education
======
* M.S. in Information and Communication Engineering, Chosun University, Gwangju, South Korea, 2025  
* B.S. in Computer Science, University of Peshawar, Peshawar, Pakistan, 2022

Work experience
======
* 2023 – 2025: Research Assistant  
  * Chosun University, Gwangju, South Korea  
  * Worked on medical image classification and detection using deep learning (Transformers, CNNs), manuscript writing, benchmarking, and collaborative research.

* Feb 2023 – Aug 2023: Research Assistant  
  * University of Peshawar, Pakistan  
  * Wireless Sensor Networks, anomaly detection, and machine learning for missing data imputation.

* Jun 2022 – Feb 2023: Machine Learning Intern  
  * REBLUE Software Company, Peshawar, Pakistan  
  * Developed image classification models, data preprocessing pipelines, and contributed to breast cancer detection systems using Python, scikit-learn, and NumPy.

Skills
======
* Computer Vision:
  * Image Classification, Detection, Segmentation
* Deep Learning:
  * Transformers, CNNs, Diffusion Models, Multi-scale learning
* Frameworks & Tools:
  * PyTorch, TensorFlow, Huggingface, Jupyter Notebook, scikit-learn, NumPy, OpenCV, timm, CUDA
* Others:
  * Data Preprocessing, Data Visualization, Explainable AI (Grad-Cam)

Publications
======
<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

Conference Presentations
======
<ul>{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}</ul>

Awards
======
* Best Paper Award, IEIE 34th AI Conference, Seoul, South Korea
* Foreign Excellence Scholarship, Chosun University, Gwagnju
* Distinction holder in B.S, University of Peshawar, Pakistan
* Certificate of Excellence – Inter-Semester AI Quiz Competition, University of Peshawar, Pakistan

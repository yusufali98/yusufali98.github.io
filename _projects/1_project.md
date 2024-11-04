---
layout: page
title: CoRL 2023
description: Large Vision-Language Models as Embodied Agents
img: assets/img/corl_img.jpg
importance: 1
category: work
related_publications: true
---

In this project, we showcase the effectiveness of using a language-driven module for the task of open-vocabulary object navigation in a never-before-seen, real-world environment on a real LoCoBot. Specifically, we finetune a recent large VLM (LLaVa-v1.5) to efficiently select subgoals which lead to the query open-vocabulary object. The LLaVa-v1.5 model is finetuned using LoRA on a dataset of GPT-4V generated multi-turn dialogue exchanges to find target objects in real world images collected by the robot. Our method uses natural language inputs to guide the robot to find new objects and leverages open-vocabulary detectors such as OWL-ViT for reliable navigation routines.


<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/corl_demo1.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/corl_demo2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div> -->

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
     {% include figure.liquid loading="eager" path="assets/img/corl_demo1.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Existing issue in leveraging VLMs for embodied navigation 
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
     {% include figure.liquid loading="eager" path="assets/img/corl_demo2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overall pipeline of our proposed solution
</div>

 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/corl_robot_video_small.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
    1x Demonstration video of running LoRA finetuned LLaVa-v1.5 online on real robot (Model inference offloaded to cluster in real-time)
</div>

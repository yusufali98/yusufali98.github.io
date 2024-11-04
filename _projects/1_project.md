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


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/corl_demo1.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/corl_demo2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Existing issue in leveraging VLMs for embodied navigation . Right : Overall pipeline of our proposed solution
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <video class="img-fluid rounded z-depth-1" controls>
            <source src="assets/video/corl_robot_video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
</div>
<div class="caption">
    Demonstration video of running VLMs on real robot.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}

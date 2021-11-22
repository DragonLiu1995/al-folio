---
layout: page
title: Multi-instrumentalist Net
description: Kun Su*, <b>Xiulong Liu*</b>, Eli Shlizerman <b>Under revision and submission</b>
img: assets/img/mi_net_teaser.png
importance: 1
category: work
---

<!-- Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/1.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/3.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/5.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div> -->


<button onclick="location.href='https://www.youtube.com/watch?v=yo5OZKBbBh4'" type="button">
         Video</button>
<button onclick="location.href='https://arxiv.org/abs/2012.03478'" type="button">
       Paper</button>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/minet_system.png title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b>a novel system that takes as an input body movements of a musician playing a musical instrument and generates music in an unsupervised setting</b>
</div>

<h3><b>Abstract</b></h3>
We propose a novel system that takes as an input body movements of a musician playing a musical instrument and generates music in an unsupervised setting. Learning to generate multi-instrumental music from videos without labeling the instruments is a challenging problem. To achieve the transformation, we built a pipeline named 'Multi-instrumentalistNet' (MI Net). At its base, the pipeline learns a discrete latent representation of various instruments music from log-spectrogram using a Vector Quantized Variational Autoencoder (VQ-VAE) with multi-band residual blocks. The pipeline is then trained along with an autoregressive prior conditioned on the musician's body keypoints movements encoded by a recurrent neural network. Joint training of the prior with the body movements encoder succeeds in the disentanglement of the music into latent features indicating the musical components and the instrumental features. The latent space results in distributions that are clustered into distinct instruments from which new music can be generated. Furthermore, the VQ-VAE architecture supports detailed music generation with additional conditioning. We show that a Midi can further condition the latent space such that the pipeline will generate the exact content of the music being played by the instrument in the video. We evaluate MI Net on two datasets containing videos of 13 instruments and obtain generated music of reasonable audio quality, easily associated with the corresponding instrument, and consistent with the music audio content.
<br><br>

<!-- <div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/6.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% responsive_image path: assets/img/11.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
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
        {% responsive_image path: assets/img/6.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% responsive_image path: assets/img/11.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %} -->

---
layout: page
title: How does it sound
description: <b>Xiulong Liu*</b>, Kun Su*, Eli Shlizerman <b>NEURIPS 2021</b>
img: assets/img/rhythmic_teaser.png
importance: 1
category: work
---

<button onclick="location.href='https://www.youtube.com/watch?v=l2gNixyX8_8'" type="button">
         Video</button>
<button onclick="location.href='https://openreview.net/forum?id=JuNatTaGZ6J'" type="button">
       Paper</button>

<div class="row">
   <div class="col-sm mt-3 mt-md-0">
       {% responsive_image path: assets/img/rhythmic_system.png title: "example image" class: "img-fluid rounded z-depth-1" %}
   </div>
</div>
<div class="caption">
   <b>RhythmicNet: it takes as an input a video which includes human movements and generates a soundtrack for it.</b>
</div>

<h3><b>Abstract</b></h3>
One of the primary purposes of video is to capture people and their unique activities. It is often the case that the experience of watching the video can be enhanced by adding a musical soundtrack that is in-sync with the rhythmic features of these activities. How would this soundtrack sound? Such a problem is challenging since little is known about capturing the rhythmic nature of free body movements. In this work, we explore this problem and propose a novel system, called 'RhythmicNet', which takes as an input a video which includes human movements and generates a soundtrack for it. RhythmicNet works directly with human movements by extracting skeleton keypoints and implements a sequence of models which translate the keypoints to rhythmic sounds.
RhythmicNet follows the natural process of music improvisation which includes the prescription of streams of the beat, the rhythm and the melody. In particular, RhythmicNet first infers the music beat and the style pattern from body keypoints per each frame to produce rhythm. Next, it implements a transformer-based model to generate the hits of drum instruments and implements a U-net based model to generate the velocity and the offsets of the instruments. Additional types of instruments are added to the soundtrack by further conditioning on the generated drum sounds. We evaluate RhythmicNet on large scale datasets of videos that include body movements with inherit sound association, such as dance, as well as 'in the wild' internet videos of various movements and actions. We show that the method can generate plausible music that aligns well with different types of human movements.

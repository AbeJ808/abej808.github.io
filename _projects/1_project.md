---
layout: page
title: Binary Clock
description: A beautifully inconvinent way of keeping time
img: assets/img/binaryclock1.jpg
importance: 1
category: personal projects
related_publications: false
---

This was one of my first personal projects at Georgia Tech. It was a fun way to get to know the makerspaces and gain some experience with their tools. I soldered the protoboard, laser cut the wooden face plate, and 3D printed the plastic casing. It was also the first time I learned what happens when you short VDD to GND, a mistake I swore I’d never make again (I absolutely made that mistake again). 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/BinaryClockDiagram.jgp" title="Reading a Bindary Clock" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/clockface.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Each column of LEDs on a binary clock represents the respective hours minutes or seconds place in an HH:MM:SS format. The digit in each place is the binary number represented by the lit LEDs in that column, with the least significant bit on the bottom. For example, the time shown on the right is 15:02:52.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/clockfusion.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/clockcircutry.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
     <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/frontofbareclockface.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The case I designed in Fusion360. The circuitry itself I soldered onto a protoboard including a real-time clock, arduino nano, and a few dozen LEDs and resistors. 
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/binaryclock1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The result is this cool desk piece that makes telling the time just that little bit harder, but certainly much more interesting. 
</div>

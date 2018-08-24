# Documentation

## Fonts & Typography

Metaphor uses the following fonts:

*   ATCOverlook - Regular
*   _ATCOverlook - Regular Italic_
*   **ATCOverlook - Bold**
*   **_ATCOverlook - Bold Italic_**
*   <span class="font-display">FSLola - Bold</span>

Please add the following line of code to the of your document to improve loading times:

    <link rel="preload" href="fonts/ATCOverlook-Regular.woff2" as="font" type="font/woff2" crossorigin>


ATCOverlook is the default font. You can make use of it's variants with the  tags in your markup, or by using **font-weight:700** or **font-weight:bold** or **font-style:italic** in your CSS or use the bootstrap-built-in classes **.font-weight-bold** and **.font-italic**.

To use <span class="font-display">FSLola Bold</span>, add a class of **.font-display** in your markup, or utilize the variable **$font-family-display** in your Sass files.  

## Timeline

By default, the dots associated with each timeline item are centered. If you want the dots to be top-aligned, you can add a modifier class of <strong class="bg-info">.timeline--align-top</strong> to the parent &lt;ul&gt;. You can also override the dot alignment of any individual item by adding the following modifier classes to the &lt;ul&gt; element:

<strong class="bg-info">
.timeline-event--align-top<br> 
.timeline-event--align-center<br>
.timeline-header--align-top<br>
.timeline-event--align-center
</strong>

<div class="row"> 
<div class="col-sm-6">
<h5>Timeline (default)</h5>
<ul class="timeline">
<li class="timeline-header">
<strong>May 2016 - Steven Kitzes - MS Computer Science</strong><br>
<a href=""><em>A Comparative Study of Asynchronous Performance in NodeJS</em></a><br>
<span>Committee Chair: A. Kaplan. Committee Members: J. Weigley and S. Fitzgerald.</span>
</li>


<li class="timeline-event">
<strong>12/12/12 - Really Long Title For This Research Publicaiton</strong>
</li>

<li>
Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corrupti culpa laudantium veniam nisi ea, maiores impedit nulla facilis beatae provident, sint expedita. Ab dolore sed sit nesciunt maiores doloribus minima! Ab consectetur adipisicing elit.
</li>

<li class="timeline-event">Thing Another Thing  <br>thing foo bar<br>another another foobar</li>

<li class="timeline-event timeline-event--align-top">Thing Another Thing thing <br>foo bar<br>another another foobar</li>
</ul>
</div>
<div class="col-sm-6">
<h5>Timeline (dots top aligned)</h5>
<ul class="timeline timeline--align-top">
<li class="timeline-header">
<strong>May 2016 - Steven Kitzes - MS Computer Science</strong><br>
<a href=""><em>A Comparative Study of Asynchronous Performance in NodeJS</em></a><br>
<span>Committee Chair: A. Kaplan. Committee Members: J. Weigley and S. Fitzgerald.</span>
</li>


<li class="timeline-event">
<strong>12/12/12 - Really Long Title For This Research Publicaiton</strong>
</li>

<li>
Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corrupti culpa laudantium veniam nisi ea, maiores impedit nulla facilis beatae provident, sint expedita. Ab dolore sed sit nesciunt maiores doloribus minima! Ab consectetur adipisicing elit.
</li>

<li class="timeline-event">Thing Another Thing  <br>thing foo bar<br>another another foobar</li>

<li class="timeline-event timeline-event--align-center">Thing Another Thing thing <br>foo bar<br>another another foobar</li>
</ul>
</div>
</div>
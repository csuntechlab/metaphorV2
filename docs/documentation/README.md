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


ATCOverlook is the default font. You can make use of it's variants with **&lt;strong&gt;**, **&lt;b&gt;**, **&lt;em&gt;**, and **&lt;i&gt;** tags in your markup, or by using **font-weight:700** or **font-weight:bold** or **font-style:italic** in your CSS or use the bootstrap-built-in classes **.font-weight-bold** and **.font-italic**.

To use <span class="font-display">FSLola Bold</span>, add a class of **.font-display** in your markup, or utilize the variable **$font-family-display** in your Sass files.  

## Timeline

A custom component intended to be used to display the passage of time.

<div class="row"> 
<div class="col-sm-6">
<h3 class="mb-3">Timeline (default)</h3>
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
<h3 class="mb-3">Timeline (dots top aligned)</h3>

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

    //timeline (default)
    <ul class="timeline">
    <li class="timeline-header"><strong>What</strong> Lorem Ipsum Foobar</li>
    <li class="timeline-event"><strong>Thing</strong> Another Thing thing <br>foo bar</li> 
    <li>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corrupti culpa laudantium veniam nisi ea, maiores impedit nulla facilis beatae provident, sint expedita. Ab dolore sed sit nesciunt maiores doloribus minima! Ab consectetur adipisicing elit. </li> 
    <li class="timeline-event timeline-event--align-top"><strong>That</strong> Metaphor Foo Thing</li> 
    </ul>

    //timeline (dots top aligned)
    <ul class="timeline timeline--align-top">
    <li class="timeline-header"><strong>What</strong> Lorem Ipsum Foobar</li>
    <li class="timeline-event"><strong>Thing</strong> Another Thing thing <br>foo bar</li> 
    <li>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corrupti culpa laudantium veniam nisi ea, maiores impedit nulla facilis beatae provident, sint expedita. Ab dolore sed sit nesciunt maiores doloribus minima! Ab consectetur adipisicing elit. </li> 
    <li class="timeline-event timeline-event--align-center"><strong>That</strong> Metaphor Foo Thing</li> 
    </ul>

By default, the dots associated with each timeline item are centered. If you want the dots to be top-aligned, you can add a modifier class of <strong class="bg-info">.timeline--align-top</strong> to the parent &lt;ul&gt;. You can also override the dot alignment of any individual item by adding the following modifier classes to the &lt;ul&gt; element:

<strong class="bg-info">
.timeline-event--align-top<br> 
.timeline-event--align-center<br>
.timeline-header--align-top<br>
.timeline-event--align-center
</strong>

## Navbar

The metaphor navbar uses the same structure as the [standard bootstrap navbar](https://getbootstrap.com/docs/4.1/components/navbar/). Just add a class of <strong class="bg-info">.navbar-metaphor</strong> to the parent  &lt;nav&gt; for the csun branded styles to take affect.

The default background color is white. For different background colors, add the following modifier classes to the parent &lt;nav&gt;

<strong class="bg-info">
.navbar-metaphor--light<br>
.navbar-metaphor--dark<br>
.navbar-metaphor--black
</strong>


Just like the standard bootrap navbar, you can add class of <strong class="bg-info">.navbar-expand-{breakpoint}</strong> to the parent &lt;nav&gt; in order to set the breakpoint which the hamburger menu appears/disapears

<nav class="navbar navbar-metaphor navbar-expand-sm">
<a class="navbar-brand" href="#">
<span class="sr-only">CSUN Logo</span>

<span class="navbar-brand__subbrand">
    MetaLab
    <small>Beta</small>
</span>

</a>
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
<span class="navbar-toggler-icon"></span>
</button>
<div class="collapse navbar-collapse justify-content-end" id="navbarNavAltMarkup">
<div class="navbar-nav text-center">
    <a class="nav-item nav-link active" href="#">Home</a>
    <a class="nav-item nav-link" href="#">Features</a>
    <a class="nav-item nav-link" href="#">Pricing</a>
</div>
</div>
</nav>

<nav class="navbar navbar-metaphor navbar-metaphor--light navbar-expand-md">
<a class="navbar-brand" href="#">
<span class="sr-only">CSUN Logo</span>

<span class="navbar-brand__subbrand">
MetaLab
<small>Beta</small>
</span>

</a>
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup2" aria-controls="navbarNavAltMarkup2" aria-expanded="false" aria-label="Toggle navigation">
<span class="navbar-toggler-icon"></span>
</button>
<div class="collapse navbar-collapse justify-content-end" id="navbarNavAltMarkup2">
<div class="navbar-nav text-center">
<a class="nav-item nav-link active" href="#">Home</a>
<a class="nav-item nav-link" href="#">Features</a>
<a class="nav-item nav-link" href="#">Pricing</a>
</div>
</div>
</nav>

<nav class="navbar navbar-metaphor navbar-metaphor--dark navbar-expand-lg">
<a class="navbar-brand" href="#">
<span class="sr-only">CSUN Logo</span>

<span class="navbar-brand__subbrand">
MetaLab
<small>Beta</small>
</span>

</a>
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup3" aria-controls="navbarNavAltMarkup3" aria-expanded="false" aria-label="Toggle navigation">
<span class="navbar-toggler-icon"></span>
</button>
<div class="collapse navbar-collapse justify-content-end" id="navbarNavAltMarkup3">
<div class="navbar-nav text-center">
<a class="nav-item nav-link active" href="#">Home</a>
<a class="nav-item nav-link" href="#">Features</a>
<a class="nav-item nav-link" href="#">Pricing</a>
</div>
</div>
</nav>

<nav class="navbar navbar-metaphor navbar-metaphor--black navbar-expand-xl">
<a class="navbar-brand" href="#">
<span class="sr-only">CSUN Logo</span>

<span class="navbar-brand__subbrand">
MetaLab
<small>Beta</small>
</span>

</a>
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup4" aria-controls="navbarNavAltMarkup4" aria-expanded="false" aria-label="Toggle navigation">
<span class="navbar-toggler-icon"></span>
</button>
<div class="collapse navbar-collapse justify-content-end" id="navbarNavAltMarkup4">
<div class="navbar-nav text-center">
<a class="nav-item nav-link active" href="#">Home</a>
<a class="nav-item nav-link" href="#">Features</a>
<a class="nav-item nav-link" href="#">Pricing</a>
</div>
</div>
</nav>

    <nav class="navbar navbar-metaphor navbar-metaphor--light navbar-expand-md">
      <a class="navbar-brand" href="#">
        <span class="sr-only">CSUN Logo</span>
        <span class="navbar-brand__subbrand">
          MetaLab
          <small>Beta</small>
        </span>
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup2" aria-controls="navbarNavAltMarkup2" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNavAltMarkup2">
        <div class="navbar-nav text-center">
          <a class="nav-item nav-link active" href="#">Home</a>
          <a class="nav-item nav-link" href="#">Features</a>
          <a class="nav-item nav-link" href="#">Pricing</a>
        </div>
      </div>
    </nav>


## Nav

The metaphor navs uses the same structure as the [standard bootstrap nav](https://getbootstrap.com/docs/4.1/components/navs/). Just add a class of <strong class="bg-info">.nav-metaphor</strong> to the parent &lt;ul&gt; for the csun branded styles to take affect.

Just like the standard bootrap navbar, the nav component can be <strong class="bg-warning">horizontaly aligned (row nav)</strong> or <strong class="bg-warning">verticaly aligned (column nav)</strong>. You can make the same nav element appear horizontally on some viewports and vertically on other viewports by adding a modifier class (<strong class="bg-info">such as .flex-{breakpoint}-column</strong>) to the parent &lt;ul&gt;

For the horizontal nav, you can force the nav items to extend the full available width. Just add the class of <strong class="bg-info">.flex-fill</strong> (or <strong class="bg-info">.flex-{breakpoint}-fill</strong> if the nav is vertical on some viewports) to each .nav-item (should be combined with class of .text-center or .text-{breakpoint}-center).

You can add a class of <strong class="bg-info">.nav-pills</strong> to the parent &lt;ul&gt; for the active nav-item to have a gray background for highlighting.

<div class="row">
    <div class="col-sm-2">
    <h5 class="mb-3"><br>Column Nav</h5>
    <ul class="nav flex-column nav-metaphor">
        <li class="nav-item">
        <a class="nav-link active" href="">Active</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
    </ul>
</div>

<div class="col-sm-2">
    <h5 class="mb-3">Column Nav with .nav-pills</h5>
    <ul class="nav flex-column nav-metaphor nav-pills">
        <li class="nav-item">
        <a class="nav-link active" href="">Active</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
    </ul>
</div>

<div class="col-sm-8">
    <br>
    <h5 class="mb-3">Row Nav</h5>
    <ul class="nav nav-metaphor">
        <li class="nav-item">
        <a class="nav-link active" href="">Active</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item">
        <a class="nav-link" href="">Link</a>
        </li>
    </ul>
    <h5 class="mb-3 mt-5">Row Nav - justified</h5>
    <ul class="nav nav-metaphor">
        <li class="nav-item flex-fill text-center">
        <a class="nav-link active" href="">Active</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
    </ul>
    <h5 class="mb-3 mt-5">Row Nav - justified with .nav-pills</h5>
    <ul class="nav nav-metaphor nav-pills">
        <li class="nav-item flex-fill text-center">
        <a class="nav-link active" href="">Active</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
        <li class="nav-item flex-fill text-center">
        <a class="nav-link" href="">Link</a>
        </li>
    </ul>
    </div>
</div>

    //column nav with nav-pills
    <ul class="nav flex-column nav-metaphor nav-pills"> 
        <li class="nav-item"> <a class="nav-link active" href="">Active</a> </li> 
        <li class="nav-item"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item"> <a class="nav-link" href="">Link</a> </li> 
    </ul>

    //row nav justifed
    <ul class="nav nav-metaphor"> 
        <li class="nav-item flex-fill text-center"> <a class="nav-link active" href="">Active</a> </li> 
        <li class="nav-item flex-fill text-center"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item flex-fill text-center"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item flex-fill text-center"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item flex-fill text-center"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item flex-fill text-center"> <a class="nav-link" href="">Link</a> </li> 
        <li class="nav-item flex-fill text-center"> <a class="nav-link" href="">Link</a> </li> 
    </ul>

## Rise Arrow

The central graphic element around the CSUN concept is the Rise Arrow. This arrow helps visualize the key message: Through CSUN, we all rise. 

<br>

<div class="rise-arrow">
</div>
<br>

    <div class="rise-arrow">
    </div>

## Badges

The <strong class="bg-info">.badge-outline-{theme-color}</strong> is custom to metaphor. The default badge is a standard bootstrap component (with metaphor colors applied instead of the default bootstrap colors).

<div class="row">
    <div class="col-6">
    <h5>Badges (default)</h5>
    <ul class="list-unstyled">
        <li>
        <span class="badge badge-success">Web Development</span>
        </li>
        <li>
        <span class="badge badge-primary">Programming Languages</span>
        </li>
        <li>
        <span class="badge badge-secondary">Parallel and Distributed Programming</span>
        </li>
        <li>
        <span class="badge badge-info">Lorem Ipsum</span>
        </li>
        <li>
        <span class="badge badge-warning">Metaphor</span>
        </li>
        <li>
        <span class="badge badge-light">Light Badge</span>
        </li>
        <li>
        <span class="badge badge-dark">Dark Badge</span>
        </li>
    </ul>
    </div>
    <div class="col-6">
    <h5>Badges (outline)</h5>
    <ul class="list-unstyled">
        <li>
        <span class="badge badge-outline-success">Web Development</span>
        </li>
        <li>
        <span class="badge badge-outline-primary">Programming Languages</span>
        </li>
        <li class="bg-primary p-1 mt-1 mb-1">
        <span class="badge badge-outline-secondary">Parallel and Distributed Programming</span>
        </li>
        <li>
        <span class="badge badge-outline-info">Lorem Ipsum</span>
        </li>
        <li>
        <span class="badge badge-outline-warning">Metaphor</span>
        </li>
        <li class="bg-dark p-1 mt-1 mb-1">
        <span class="badge badge-outline-light">Light Badge</span>
        </li>
        <li>
        <span class="badge badge-outline-dark">Dark Badge</span>
        </li>
    </ul>
    </div>
</div>

    //badge default
    <span class="badge badge-success">Web Development</span>
    <span class="badge badge-primary">Programming Languages</span>
    <span class="badge badge-secondary">Parallel and Distributed Programming</span>
    <span class="badge badge-info">Lorem Ipsum</span>
    <span class="badge badge-warning">Metaphor</span>
    <span class="badge badge-light">Light Badge</span>
    <span class="badge badge-dark">Dark Badge</span>

    //badge outline
    <span class="badge badge-outline-success">Web Development</span>
    <span class="badge badge-outline-primary">Programming Languages</span>
    <span class="badge badge-outline-secondary">Parallel and Distributed Programming</span>
    <span class="badge badge-outline-info">Lorem Ipsum</span>
    <span class="badge badge-outline-warning">Metaphor</span>
    <span class="badge badge-outline-light">Light Badge</span>
    <span class="badge badge-outline-dark">Dark Badge</span>


## Icon Library - Font Awesome

<i class="fas fa-user"></i>

## Datepicker

Include the datepicker.js file (included with MetaphorV2). Initialize with <code>$('.date').datepicker();</code> The datepicker is accessible. 

<div class="form-group">
    <label for="date1">Chose a Date:</label>
    <input class="date form-control" id="date1" type="text" placeholder="mm/dd/yy" title="format: mm/dd/yy"/>
</div>
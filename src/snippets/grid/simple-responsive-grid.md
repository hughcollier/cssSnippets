---
title: An incredibly simple responsive grid.
---

This is such a cool way to create a simple grid! With only the following CSS set on the parent we now have a responsive grid (no need for any media queries) that will create a grid with equal columns with each column with a minimum width of 250px. Nice!


<pre>
<code class="language-css line-numbers">
  
.card-container {
  display: grid; 
  grid-template-columns: repeat(auto-fit, minmax(250px,1fr)); 
  gap: 1rem;
}

</code>
</pre>

<div class="demo">
  <div id="card-container">
    <div class="card card-1"></div>
    <div class="card card-2"></div>
    <div class="card card-3"></div>
    <div class="card card-4"></div>
    <div class="card card-5"></div>
    <div class="card card-6"></div>
    <div class="card card-7"></div>
    <div class="card card-8"></div>
    <div class="card card-9"></div>
  </div>
</div>

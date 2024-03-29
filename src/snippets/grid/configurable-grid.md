---
title: A more configurable grid.
---

In this example we use `display: grid` on the container to setup a our basic grid for mobile and then use a media query to target larger screen sizes.

This example shows how we can place our elements more precisely by individually specifying each child's location within the grid we have defined.

<pre>
		<code class="language-css line-numbers">

		#card-container-2 {
			display: grid;
			gap: 1rem;
		}
		
		@media (min-width: 40em) {
			#card-container-2 {
				grid-template-columns: repeat(3, 1fr);
			}
			#card-container-2 .card-1 {
				grid-column-start: 1;
				grid-column-end: 3;
			}
			#card-container-2 .card-7 {
				grid-column-start: 2;
				grid-column-end: 4;
			}
		}

			</code>
		</pre>

<div class="demo">
  <div id="card-container-2">
    <div class="card card-1"></div>
    <div class="card card-2"></div>
    <div class="card card-3"></div>
    <div class="card card-4"></div>
    <div class="card card-5"></div>
    <div class="card card-6"></div>
    <div class="card card-7"></div>
  </div>
</div>
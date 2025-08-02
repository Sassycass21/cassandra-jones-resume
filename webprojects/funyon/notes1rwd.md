## viewport meta element with standard parameters
<meta name="viewport" content="width=device-width, initial-scale=1">
 add user-scalable=no toto prevent user from zooming in and out 

##Viewport units
<!DOCTYPE html>
<html>
   <title>Viewport units</title>
   <style type="text/css">

#first {
   background: cornflowerblue;
   width: 80vw; 
}

#second {
   background: lightgreen;     
   height: 20vh;
}

#third {
   background: mistyrose;    
   width: 50vmin;
}
   </style>
   <body>
      <div id="first">First</div>
      <div id="second">Second</div>
      <div id="third">Third</div>
   </body>
</html>
The First <div> has a width of 80vw, which is 80% of the viewport width.
The First <div> width grows wider as the browser's viewport is made wider.
The Second <div> has a height of 20vh, which is 20% of the viewport height.
Second <div> height increases as the viewport height increases.
The Third <div> has a width of 50vmin, which is 50% of the viewport width when the viewport width < height.
50vmin is 50% of the viewport height when the viewport width > height.

## Evaluating Media Queries
<!-- CSS media query on a link element -->
<link rel="stylesheet"
   media="print and (min-width: 400px)" 
   href="styles.css">

<!-- CSS media query in a stylesheet -->
<style>
@media screen and (max-width: 800px) {
  .proposal {
      width: 350px;
  }
}
</style>

A webpage with media queries is being viewed on a mobile device with a viewport that is 500px wide.
The link element defines a media query: Is the webpage being printed and the viewport's width ≥ 400 pixels?
The "print" media type is false because the webpage is displayed on a mobile device. The media query does not match, so styles.css is not downloaded.
The stylesheet uses a media query: Is the webpage displayed on a viewport that is ≤ 800 pixels wide?
The "screen" media type is true and 500px ≤ 800px, so the media query matches. The .proposal class is defined.


## Art Direction for Various Screen Sizes
<picture>
   <source media="(min-width: 600px)"
           srcset="dog-wide.jpg">
   <source media="(min-width: 400px)"
           srcset="dog.jpg">
   <img src="dog-narrow.jpg"
           alt="Dog">
</picture>

Three browsers have different widths. All three browsers read the <picture> element.
Browser with width = 350px does not match media query, requests dog-narrow.jpg.
Browser with width = 400px requests dog.jpg.
Browser with width = 1000px requests dog-wide.jpg.
Playing step 1: Three browsers have different widths. All three browsers read the <picture> element. Step finished playing


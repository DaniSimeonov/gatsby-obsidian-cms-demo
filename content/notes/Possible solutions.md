# Interactive expandable tree diagram
![[interactive-flowchart.mp4]]

## Possible approaches

- Plain HTML and CSS
- SVG animations
- HTML5 2D canvas - limited browser support
- webGL - much better browser support

## Vanilla HTML and CSS
- Very difficult (dare I say impossible) to have relational hierarchical structure
- Can get links but when adding animations unable to keep correct links and positions.
- More familiar than other options at least, but not robust enough to do what we need it to do.

![[html-css-static.mp4]]
![[html-css-moving.mp4]]

 ## SVG formatting 
- Libraries like [d3.js](https://d3js.org/).
- Very difficult to work around preprogrammed animations and movements.  i.e. tree diagrams are very easy to make with a lot of options, but I have not been able to find an example or documentation on how to  add html or have nodes expand while keeping links correct.
- 

![[d3-tree.mp4]]
![[d3-treebox.mp4]]

## HTML5 Canvas
- Only available on major browsers - Firefox, Chrome, IE, Safara, Opera, Edge, Konqueror. 
- Have not found any free libraries that come anything clsoe to what we need
- [KeyLines](https://cambridge-intelligence.com/)
- [Ogma](https://doc.linkurio.us/ogma/latest/)
- [yFiles](https://www.yworks.com/products/yfiles)
-  [goJS](https://gojs.net/latest/index.html)

yFiles has clients like Google and Microsoft, but with a [license structure](https://www.yworks.com/products/yfiles-for-html/pricing) to match.

Ogma and Keylines required direct contact for pricing.

#### Commercial Library of Choice - goJS
All of the commerical libraries can do almost anything I think. I need a few days per library just to dig into documetnation and use cases.

I received 2 responses from goJS support in one day, and they are priced at about 1/6th on average compared to yFiles. They have like 50 samples on their site and their API documentation is beyond meticulous. 

![[goJS-expand.mp4]]
![[goJS-another.mp4]]

## webGL
- More modern and 3D focused rendering engine, but also does 2D perfectly fine.
- I was not able to find a single library focused solely on webGL doing data driven application solutions like we need. yWorks has an insane line up of functionality, even shifting through canvas, SVG and webGL based on performance capabilities based on your use case. 
- [Pixi.js](https://www.pixijs.com/) would be preferred library, and is free (Draws in webGL and in canvas). But again, I found nothing even remotely similar to what we are trying to do, so there will be a lot of custom work even if the library is built for animation.

## Performance 
When comparing the performance of webGL, HTML5 canvas and SVG, everyone sings a different song. Most of the debate is for either super simple applications or super complex applications with 10s or 100s of data points. You can find a comprehensive comparison [here](https://www.yworks.com/blog/svg-canvas-webgl) with a live demo [here](https://live.yworks.com/demos/view/largegraphs/)]


## End Notes
Please realise that each of these topics are a week of reseach on their own, if not more. I am now at the point that I need hours of fiddling and further hands on with relevant libraries and experimenting to become more familiar with them and give more comprehensive insight.





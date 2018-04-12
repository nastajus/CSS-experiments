![CSS negative space images](https://github.com/nastajus/CSS-experiments/raw/master/negative-space-images.png "Skateboard, Shoe sole, Tennis racket")

# CSS Experiments

### 1. CSS property display:flex

Basic usage: Flex, a.k.a. flexible box, or flexbox, is a newer way to control layouts used in more [recent browsers](http://caniuse.com/#feat=flexbox). It's a great enhancement for [divs](https://www.sitepoint.com/community/t/div-background-color/6709), which are used to control webpage flow layout in the form of blocks. Previously before flex, people hardcoded with [absolute pixel positions](http://stackoverflow.com/questions/5161046/html-div-positions-and-display), this wasn't scalable.  Now with flex, minimum heights and widths can be specified, making it much easier. 

###### References on how flex works

1/6: https://www.youtube.com/watch?v=sewV3LsmoXI&index=22&list=PL942738B74C08BF97

2/6: https://www.youtube.com/watch?v=0i7Xb22zzQM&list=PL942738B74C08BF97&index=24

3/6: https://www.youtube.com/watch?v=KCZdKnP5PHo&list=PL942738B74C08BF97&index=23



### 2. CSS shapes positioned

These shapes are done built of pure CSS, with only empty divs as the only [HTML elements](http://www.w3schools.com/html/html_elements.asp). The only colors used are black and white, permitting the art style [form and counterform](http://www.gdbasics.com/html/figure/figure.html) to be used. Everything is [absolute positioned](https://css-tricks.com/almanac/properties/p/position/), so lot of tweaking of exact pixel placements was done.   The goal was to push my design capability boundaries.  

###### Skateboard: 
**Time:** 3 hours
**Features:** Rectangles, triangles, circles. Elliptical curves, circular curves.

Interestingly, the board is composed of two rectangles overlapping of differing dimensions, so that two distinct curves could be made with little complexity. (The simple beauty of black & white design shines here.) Layered on top are the wheels, and wheel hangers, but in white creating [negative space](https://en.wikipedia.org/wiki/Negative_space), with the corners curved with an equal radius on all sides (so circular corners). To get the triangular effect, used in part of the wheel hanger ("truck"), an interesting "abuse" or "hack" was used, involving pure borders and no body size, so to say. The pure circles for screws, those were really rectangles originally too, but those just have a maximum radius set, appearing as circles. 

###### Shoe Sole: 
**Time:** 2 hours
**Features:** Rotations. Multiple curve shapes per object. 

I made two types of treads (white lines): one fully extending past the edge of the shoe, the other terminating within. To hide the fact these were sharp rectangles rotated at various angles, the corners are completely rounded, to avoid many jaggies sticking out all over. Essentially an artistic liberty taken to compensate for the limitations of this medium.  So this went faster due to the repeating pattern, just needed to copy-paste CSS blocks for each shoe tread and tweak slightly their positions. 

###### Tennis Racket: 
**Time:** 3 hours.  *(Intended to be 1 hour, backfired due to exhaustion)* 
**Features:** Positions with rotations. Inverted curves.

I deliberately complicated this design to push my knowledge. Fully aware this would cause design consequences by rotating everything in pure CSS, I proceeded regardless. This racket presented two challenges to choose from: either make the lines (strings) of variable lengths both begin and terminate perfectly within the thin line of an oval, or I'd have to perfectly obscure the protrusions with some kind of inverted curved corner. I ended up trying and imperfectly doing both, but I learned. In essence, this object choice made clear how important the CSS `transform-origin` property is when combined with **rotation** when combined with **absolute positioning** with trying to offset equally multiple copies. My last workflow was ruined, where I simply copy-pasted my `string` classes adjusted only the `top` or `left` properties. What I learned was I could've preserved this workflow with more careful usage of `transform-origin`.



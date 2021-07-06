# CSS Transforms, Transitions, and Animations:
## CSS Transforms:

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

The `transform` property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

`div {`
  `-webkit-transform: scale(1.5);`  
     `-moz-transform: scale(1.5);`  
       `-o-transform: scale(1.5);`  
          `transform: scale(1.5);`  
`}`

## The transform property can either be :

- two dimensional 
- three dimensional

## 2D Transforms #two-dimensional-transforms:

**2D Rotate:**


The `transform` property accepts a handful of different values. 

The rotate value provides the ability to rotate an element from 0 to 360 degrees.

`.box-1 {`  
  `transform: rotate(20deg);`  
`}`  
`.box-2 {`  
  `transform: rotate(-55deg);`  
`}`  

**2D Scale**

Using the `scale` value within the `transform` property allows you to change the appeared size of an element. The default scale value is `1`, therefore any value between `.99` and `.01` makes an element appear smaller while any value greater than or equal to `1.01` makes an element appear larger.

`.box-1 {`
  `transform: scale(.75);`
`}`
`.box-2 {`
  `transform: scale(1.25);`
`}`

## 3D Transforms #three-dimensional-transforms:

**3D Rotate**

So far we’ve discussed how to rotate an object either clockwise or counterclockwise on a flat plane. With three-dimensional transforms we can rotate an element around any axes. To do so, we use three new `transform` values, including `rotateX`, `rotateY`, and `rotateZ`.


`.box-1 {`  
  `transform: perspective(200px) rotateX(45deg);`  
`}`  

**3D Scale**

By using the `scaleZ` three-dimensional transform elements may be scaled on the `z` axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale. In the demonstration below the elements are being scaled up and down on the `z` axis, however the `rotateX` value is added in order to see the behavior of the `scaleZ` value. When removing the `rotateX` in this case, the elements will appear to be unchanged.

`.box-1 {`  
  `transform: perspective(200px) scaleZ(1.75) rotateX(45deg);`  
`}`

**To more info please :[ Visit This Page](https://learn.shayhowe.com/advanced-html-css/css-transforms/#three-dimensional-transforms)**

-------

## Animations

Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

**Animations Keyframes**

To set multiple points at which an element should undergo a transition, use the `@keyframes` rule. The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

	
`@keyframes slide {`  
  `0% {`  
    `left: 0;`  
    `top: 0;`  
  `}`   
  `50% {`   
    `left: 244px;`   
    `top: 100px;`   
  `}`   
  `100% {`   
    `left: 488px;`  
    `top: 0;`   
  `}`    
`}`
					 
**To more info please :[ Visit This Page](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)**

-----





**To WOW you user :**
**[ Visit This Page](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/)**

**[ 6 Buttons animated](https://codepen.io/retyui/pen/ByoaXV/)**

**[ CSS3 Animations: Keyframes](https://codepen.io/akshaychauhan/pen/oAfae/)**

**[ 404](https://codepen.io/kieranfivestars/pen/MYdQxX/)**

**[ Pure CSS Bounce Animation](https://codepen.io/dp_lewis/pen/gCfBv/)**









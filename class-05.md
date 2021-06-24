# HTML Images, Color, Text
## HTML Images:
- ### How to add images to pages:
`<img>`:

To add an image into the page you need to use an `<img>` element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:

`src` :
This tells the browser where
it can find the image file.

`alt`:
This provides a text description of the image which describes the image if you cannot see it.

`title`:
You can also use the title
attribute with the `<img>` element to provide additional information
about the image.

`height`, `widtb`: To specify the size.

--------------------------


 ## Color:

- ### `color`: 

color names: `red`

rgb values: `rgb(255, 0, 0)`

hex codes: `#ff0000`

- ### background-color:

`background-color: rgb(200,200,200);`

- ### Opacity :

`opacity`: To opacity of an element and any of its child elements

`rgba`: allows you to specify a color

----------------------

## Text:
`font-family`:
The font-family property
allows you to specify the
typeface that should be used for any text inside the element(s) to which a CSS rule applies.

`font-size` : 
The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font.

`@font-face` : 
@font-face allows you to use
a font, even if it is not installed on the computer of the person browsing.

> Like This:    
`@font-face {
font-family: 'ChunkFiveRegular';
src: url('fonts/chunkfive.eot');}`

`font-weight` : 
The font-weight property
allows you to create bold text.

`font-style` : 
If you want to create italic text, you can use the font-style property.

`text-transform` : 
The text-transform property
is used to change the case of
text giving it.

> Like This :  
`text-transform: uppercase;`

`text-decoration` : 
Property specifies the decoration added to text.

`line-height` : 
Property to specifies the height of a line

`text-indent` : 
The text-indent property
allows you to indent the first line of text within an element.

`:hover` : This is applied when a user hovers over an element with a pointing device such as a mouse.

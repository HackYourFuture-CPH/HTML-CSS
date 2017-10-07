# Week 2

### Agenda
- Standup
- CSS Selectors
- Positioning
- Responsive design

## CSS Selectors
- Type selector
```css
div {
    background-color: red;
}
```
This selector targets ALL `div` tags in our HTML

- Class selector
```css
.container {
    background-color: red;
}
```
This selector targets all the elements (no matter the tag) that have the class attribute of container.



- Id selector
```css
#container {
    background-color: red;
}
```
This selector targets the element that have the id of "container"
Note: Remember that `id` should be used to target only one element, if you wish to target more than one element you shoudl always use classes.

- Universal selector
```css
* {
    color: red;
}
```
This selector targets ALL the tags in your HTML, it targets everything.

- Pseudo selectors:
```
:hover, :active, :focus, :first-child, and lots more!
```
You can read more about pseudo selectors available here: https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes

- `.header .callout`
Select all elements with the class name callout that are      descendants of the element with class name header.
- `.header,  .callout`
Select all elements with class name header AND select all elements with class name callout
- `.header.callout`
Select all elements with class name header and class name callout <div class=“header callout”></div>

## Exercise
Open https://codepen.io/dalsHughes/pen/wdYxNv
1. Center the title with the text “CSS selectors”
2. Change the font to Helvetica
3. Create some space (think margin) between the container div tags
4. Give the three containers padding and a lightgrey background
5. In the text-container make the span text color red
6. Lets get some space between all list elements
7. The second list should have a black border and its elements should have blue color.
8. Give the element with id a black text color
9. When hovering over the link, change the color to red
10. The second element of the lists should have a lightyellow background color

No changing html and Google is your friend!

## Document Flow

Elements can be either block or inline

- Inline elements flows horizontally
- Block elements flow vertically

ADD IMAGE

Additionally elements can be set to inline-block, which allows elements inline elements to have a height and width independent of the content.


add image

### Float

Float will pull an element either to the left or to the right.
Was designed to make text “float” around an image or a similar object.

ADD IMAGE
#### Clearfix
Floating an element takes it out of the “document flow”. I.e. non floated elements will not know where the floated element stops.

Solution:

use clear: both on the subsequent element.

ADD IMAGE

## Exercise
Build a classical site layout:

https://codepen.io/webconsult/pen/LyXzNY
ADD IMAGE

## CSS Positioning
As an addition to using floats you can use positioning for placing objects on the page.
https://codepen.io/webconsult/pen/MmzQEz

## Flexbox
Layout mode for arranging elements in containers
Accommodate HTML content on different screen sizes
Flexbox guide: https://css-tricks.com/snippets/css/a-guide-to-flexbox/

## Media queries
- Flexible width example: http://codepen.io/webconsult/pen/rmQJKE
- Responsive website example: http://codepen.io/webconsult/pen/EmOQpx
- Good example of a responsive site:
www.telmore.dk

- A media query is a way to control the presentation of content
- Used to make layouts that works on all device sizes
- Used to check width of viewport, width of device, orientation, resolution, aspect-ratio and a lot more
- To start with responsive webdesign, lets first tell the brower what width it should use: <meta name="viewport" content="width=device-width,initial-scale=1">
- This tells the browser to use the width from the device and set initial scale to 1. Scale is the initial zoom.

### Rules

- Multiple and rules
```css
@media only screen and (min-width: 320px) and (orientation: portrait) {
    color: red;
}
```
- Multiple or rules
```css
@media only screen and (min-width: 320px), (orientation: portrait) {
	color: red;
}
```
- Not rule
```css
@media only screen and not (min-width: 320px){
color: red;
}
```

### Best practice
Change media query NOT dependent on device, but when layout looks broken.
Start with the small screen first, then expand until it looks like shit. Time for a breakpoint! –Stephen Hay
Start by developing for a mobile and then add media queries as above. This is called mobile first development (and it is so hot right now!)
Worth reading: http://bradfrost.com/blog/post/7-habits-of-highly-effective-media-queries/
https://css-tricks.com/logic-in-media-queries/

## Percentages
- It is possible to use percentages as unit in margin, padding, width, height and font-size (maybe more)
- The percentage is set compared to the parent element
- If we want 4 columns next to each other, what percentage should we have?
https://codepen.io/dalsHughes/pen/bqqNeq

## Exercise
Go to http://codepen.io/dalsHughes/pen/aJWKav
- Lets start with the mobile and work out from there! (mobile first development)
- First lets give grid-item element some padding and a lightgrey background-color. And lets get some space between the grid-items.
- When expanding the window at some point instead of the grid-items laying on top of each other, let them stand next to each other as columns. Also increase the padding on the grid-item
- Add gutters (space between the columns).
- When we go very wide, change the body color to red ☺

# Frontend community
- http://shoptalkshow.com/ - Frontend podcast
- http://javascriptweekly.com/ - Frontend newsletter
- https://www.meetup.com/copenhagenjs/ - Js meetup
-

# To read for next class
[Introduction to media queries](https://teamtreehouse.com/library/css3/media-queries/introduction)
[More about media queries](https://css-tricks.com/css-media-queries/)
[HTML syntax](http://www.w3schools.com/html/html5_syntax.asp)
[Article about multiple ways to select classes and id's](https://css-tricks.com/multiple-class-id-selectors/ )
[Read about nice color combinations](http://www.colorcombos.com/index.html)

# Homework
Go to: https://codepen.io/dalsHughes/pen/RVeqKB, fork it and do the following exercise:

 - Grids exercise
    - Download the HTML and images in the folder Homework 2
    - You are going to write the CSS for this page
    - You are not allowed to change the HTML
    - The page contains two grids: the first one should work using floats, the second using flex box. Be careful not to mix the two!
    - We want the grid to look as follows:
      - On mobile phones: a two column grid, with the exception that the first item spans the full width
      - On tablets: a three column grid, with the exception that the first two items span the full width together (so first we have two columns, then after the first two items we have three columns)
      - On desktops: a four column grid, with the exception that the first item spans two columns.
    - There should be some space between the grid items
    - Make the page look beautiful by adding some more CSS! Some tips:
      - How about some nice colors, fonts, hover styles?
      - According to the grid specification, some products are bigger than others. Maybe these are "highlighted" products, so the rest of the styling could also be different.
    - BEFORE you hand it in, read [the Style guide](http://www.w3schools.com/html/html5_syntax.asp) again and check your files

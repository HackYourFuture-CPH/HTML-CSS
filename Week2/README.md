# Week 2

```
In week two we will discuss the following topics
- CSS Selectors
- Positioning
- Responsive design
```

- [CSS tricks ]https://css-tricks.com/inheriting-box-sizing-probably-slightly-better-best-practice/)
- Bookmark the sites/resources that you used that where most useful for you the last two weeks.

_Please go through the material and come to class prepared!_

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

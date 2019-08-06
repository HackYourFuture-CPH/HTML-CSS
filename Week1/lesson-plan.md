
# Exercises

Exercises made by [Niels Gregersen](https://github.com/senner007)

## Exercise 1
Create web page where you introduce yourself. It should only have a headline, an image and some text.
- Create an index.html file with only the basic structure: 

``` 
<!DOCTYPE html>
<html>
    <head>
    <title>About me</title>
    </head>

    <body>

    </body>
</html>
```
- Accomplish the above task without styling any of the elements
- Add inline styles.
- Add a reference to an external css file and transfer the styling to this file.

Does the image have an alt attribute? If not, add one.
[The alt Attribute](https://www.w3schools.com/html/html_images.asp)

## Exercise 2

Create and index.html with the follow hierarchy:

```
<div id="container">
    <div>
        <p>
            First p element in first div child
        </p>
        <p class="cool-style">
            Second p element in first div child
        </p>
    </div>
    <div>
        <ul>
            <li>
                First li element in second div child
            </li>
            <li>
                Second li element in second div child
            </li>
        </ul>
    </div>
    <div>
        <ul>
            <li>
                Li element in third div child
            </li>
        </ul>
        <p class="cool-style">
            P element in third div child
        </p>
    </div>
</div>

```
Describe the hierarchy to the person sitting next to you. Draw a visual representation of the hierarchy

Create an external main.css file and add a reference in the index.html.
Do not add ids or classes to the tags. Now add the following specific styles:

- select all elements. Add blue font color
- select all li elements. Add red font color
- select the second p element in the first div child. Add green color to the font. Hint: use the nth-child selector 
- select the li element in the third div child. remove the dot
- select the elements that have a class of 'cool-style'. Add some cool styling. 


Now add your own improved styles so the hierarchy becomes visible/obvious to the viewer.

## Exercise 3

Create an index.html with elements in the depicted hierarchy. Add ids and classes.

![alt text](https://github.com/senner007/temp/blob/master/Hierarchy-1.png "Logo Title Text 1")


## Exercise 4

You have been hired to create a website for at company. It has to have the structure that is depicted below. Hint : use the float property

![alt text](https://github.com/senner007/temp/blob/master/img_sem_elements.png "Logo Title Text 1")

- use div tags only
- use semantic tags
  
## Exercise optional 1

Play the game called CSS Diner : https://flukeout.github.io/

## Exercise optional 2

Get a head start on week 2. Learn flex-box!
Go to https://flexboxfroggy.com/


Exercises made by [Niels Gregersen](https://github.com/senner007)

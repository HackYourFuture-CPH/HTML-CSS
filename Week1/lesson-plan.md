# Lesson plan
```
> Focus on having lots of in class exercises.

> DONT teach everything, let the students investigate topics on their own aswell!

> Focus on how to read documentation, google answers and google errors!!

> Teach towards the students being able to solve the homework
```

---

- Quick introduction of mentors
- Importance of asking questions
- The division of labor between HTML and CSS
- HTML
    - WHAT IS HTML?
  	- HTML tree structure (dont go into detail about DOM, this is expalined in the js class)
    	- Parents, children, attributes
    - [Exercise 1](#exercise-1)
    - HTML TAGS
      - Standard (div, p, span, h1)
      - Semantic
    - [Code inspiration](#simple-html-page)
- Introduction to ARIA
- CSS
    - Add and remove style from a website
    - [Code inspiration teaching the below topics](#simple-css-inline)
        - CSS selectors
          - Id, class and type
          - Child: `.red-color .text`, and selector `.red-color, .text`, 
          - Pseudo selector `.red-color:hover`
          - nth-child(), sibling
    	- Specificity
        - Properties mention a few (color, width, height, etc.)
         	- Rules will be applied to ALL elements that match your selector
        - External vs inline styles vs element style
    - If time Boxmodel: border-box: width is set with the border inside! content-box, 100 px refers ONLY to the content, padding, border is on top! [Code inspiration](#box-model)
    - How to structure a CSS file
    - Naming things
 - External files: relative and absolute paths
 - Getting to know your text editor

[Exercise 2](#exercise-2), [Exercise 3](#exercise-3), [Exercise 4](#exercise-4, [Exercise optional 1](#exercise-optional-1)

# Code inspiration

## Simple html page
```
<html>
  <head>
    <title>test dom</title>
  </head>
  <body>
    <div>
      <h1>Beneath is a link to Hack Your Future:</h1>
      <a href="http://www.hackyourfuture.net/">Hack your future</a>
      <div class="hello-world-container">
        <p>
          Hello Students
        </p>
        <p>
          This is some text on a page
        </p>
      </div>
    </div>
  </body>
</html>

```

## Simple css inline

```
<html>
  <head>
    <title>
      Hack your future example
    </title>
    <style>
      p {
        font-size: 30px;
      }

      .hello {
        color: green;
      }

      .hello .blue {
        color: blue;
      }

      #orange {
        color: orange;
      }

        .hello-world-container .blue {
            color: blue;
        }

      .hello-world-container:nth-child(2) {
          background-color: pink;
      }
    </style>
  </head>
  <body>
    <div class="hello-world-container">
      <p class="hello">
        <span class="blue">
          Hello World
        </span>
      </p>
      <p>
        This is some text on a page
      </p>
      <span class="blue">Blue</span>
    </div>
  </body>
</html>

```

## Box model
Fix the last box that pops into the next line

```
<html>
    <head>
        <title>
            Hack your future example
        </title>
        <style>
        .container {
          background-color: #2766AC;
          border: 5px solid red;
          box-sizing: border-box;
          float: left;
          padding: 20px;
          width: 33%;
        }

        </style>
    </head>

    <body>
      <div class="container">
        <a href="google.com">Go to Google!</a>
      </div>
      <div class="container">
        <a href="google.com">Go to Google!</a>
      </div>
      <div class="container">
        <a href="google.com">Go to Google!</a>
      </div>
    </body>
</html>
```

OR

```
<html>
<head>
    <style>
      .box-model {
        width: 100px;
        height: 100px;
        background-color: black;
        padding: 10px;
        margin: 20px;
        border: 20px solid grey;
        box-sizing: border-box;
      }
    </style>
</head>
  <body>
    <div class="box-model"></div>
  </body>
</html>

```

# Exercises

Exercises made by [Niels Gregersen](https://github.com/senner007)

## Exercise 1

Answer the questions below using the html found beneath

```
<section>
    <div>
        <p>hello</p>
        <p>world</p>
        <a href="#">
            <ul>
                <li>Hack</li>
                <li>your</li>
                 <li>Future</li>
            </ul>
        </a>		
    </div>
</section>

```

1. The p element with the text “world” - what elements is its parent?
1. What text is written in the ul element’s second child?
1. What text is written in the div element’s first child?
1. The p element with the text world, what siblings does it have?


## Exercise 2
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
- Remember to add the styling through an external css file.

Does the image have an alt attribute? If not, add one.
[The alt Attribute](https://www.w3schools.com/html/html_images.asp)

## Exercise 3

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
Do not add ids or classes to the tags! Now add the following specific styles:

- Select all elements. Add blue font color
- Select all li elements. Add red font color
- Select the second p element in the first div child. Add green color to the font. Hint: use the nth-child selector 
- Select the elements that have a class of 'cool-style'. Add some cool styling. 

## Exercise 4
Describe when to use the following tags and what they do:
`header, footer, section, canvas, nav, article, main, audio, video`

## Exercise optional 1

Play the game called CSS Diner : https://flukeout.github.io/

Exercises made by [Niels Gregersen](https://github.com/senner007)

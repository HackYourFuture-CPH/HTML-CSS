## Homework Week 3

In the folder “wireframes” you find wireframes for a signup flow for a website that finds special deals on clothes, handbags and accessories based on users personal preferences.

The signup form is fairly complex and broken into 3 steps in order not to scare away users.

![Get to work](https://media.giphy.com/media/3og0ITQOC5wlyk8ffy/giphy.gif)

The task is to recreate this form in HTML and CSS. You should focus on using the right HTML form tags for the job, applying the general layout. There is no visual design provided, so you can choose colors etc. but no focus is put on good or bad visual design, so it is suggested that you just leave all of the form inputs with the stock styling and only try to refine this if you have completed all other parts.

Currently you are expected to create 3 separate HTML files and set up links between them using [anchor tags](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a). _(Forms cannot be sent properly using the `htmlpreview.github.io` tool, however, you can experiment with ideas to overcome this issue. We've seen people use a link-shortener like `bit.ly` to convert the `action` link to a shortlink that can accept the form submission.)_ If you feel like trying out some more techniques beyond what we've learned in class, try putting the steps into separate tabs for example by using a library. Or you can also create tabs using the [checkbox hack](https://codepen.io/te-online/pen/mdMZrwO).

There is a progress bar that will indicate how far the user is. If you have time, try to use CSS transitions to animate it so the bar goes from 0-1 on the first page, 1-2 on the second page and so on (with a smooth and nice animation).


Direct links to wireframes:

[Step 1a](https://github.com/HackYourFuture-CPH/HTML-CSS/blob/master/Week3/wireframes/Step%201a.pdf)

_(optional) [Step 1b](https://github.com/HackYourFuture-CPH/HTML-CSS/blob/master/Week3/wireframes/Step%201b.pdf)_

[Step 2](https://github.com/HackYourFuture-CPH/HTML-CSS/blob/master/Week3/wireframes/Step%202.pdf)

[Step 3](https://github.com/HackYourFuture-CPH/HTML-CSS/blob/master/Week3/wireframes/Step%203.pdf)

_(optional) [Step 4](https://github.com/HackYourFuture-CPH/HTML-CSS/blob/master/Week3/wireframes/Step%204.pdf)_

Below is an overview of the fields in the form and how they should be validated. To figure out the right regular expression pattern try searching for something like (“regex only letters”) and use something like [this website](https://regexr.com/) to test that the pattern you have found works correctly.

| Field name                   | Required | Validation criteria                                    |
|------------------------------|----------|--------------------------------------------------------|
| First name                   | yes      |                                                        |
| Last name                    | yes      |                                                        |
| Country                      | yes      |                                                        |
| Street address               | yes      |                                                        |
| Post code                    | yes      | Assume Danish address, so allow only 4 letters         |
| Profile description          | no       | Maximum 500 characters                                 |
| Shipping address             | yes      |                                                        |
| Email                        | yes      | Allow only valid email addresses                       |
| Phone                        | no       | Allow only valid phone numbers                         |
| Password                     | yes      | Minimum 10 characters, uppercase and lowercase letters |
| Password repeat              | yes      | Minimum 10 characters, uppercase and lowercase letters |
| Newsletter                   | yes      | One radio option must be selected                      |
| Kind of items                | no       | Must be possible to select 0, 1 or many options        |
| "Resemble your style" images | no       | Must be possible to select 0, 1 or many options        |
| Name on creditcard           | yes      |                                                        |
| Card type                    | yes      |                                                        |
| Credit card number           | yes      | Only numbers allowed. Exactly 16 digits                |
| Expiry month                 | yes      |                                                        |
| Expiry year                  | yes      |                                                        |
| CCV                          | yes      | Only numbers. Exactly 3 digits                         |

## Form validation *optional*
Create sensible form validation for the forms. Read up on form validation [here](https://css-tricks.com/form-validation-part-1-constraint-validation-html/).

## Hand in Homework:
- With the `https://github.com/USERNAME/hyf-homework`, find the relevant week number
- Now upload your homework files to the repo 
- If you forgot how to do that, check it out [here](../Week1/homework.md#hand-in-homework)
- Post your index.html file on your class' Slack channel in this format: https://htmlpreview.github.io/?https://github.com/YOUR_ACCOUNT/hyf-homework/blob/master/html-css/week1/index.html

## Send us feedback ❤️
Please, take a few minutes to give us feedback about the module by filling out the survey [here](https://forms.gle/Emxh1kqmCL6ybUeh7). 

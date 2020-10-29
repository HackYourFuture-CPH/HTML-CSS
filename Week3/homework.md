## Homework Week 3

In the folder “wireframes” you find wireframes for a signup flow for a website that finds special deals on clothes, handbags and accesories based on users personal preferences.

The signup form is fairly complex and broken into 4 steps in order not to scare away users.

![Get to work](https://media.giphy.com/media/3og0ITQOC5wlyk8ffy/giphy.gif)

The task is to recreate this form in HTML and CSS. You should focus on using the right HTML form widgets for the job, applying the general layout. There is no visual design provided, so you can choose colors etc. but no points are awarded for good or bad design so it is suggest that you just leave all of the form input with the stock styling and only try to refine this if you have completed all other tasks.

Currently you are expected to create 4 separate HTML files and set up links between them using anchor (<a>) tags. If you feel like trying out some more techniques learned in class today, try instead putting the 4 different form steps into tabs using the library we learned to use today. Or you can also create tabs using the checkbox hack. 

There is a progress bar that will indicate how far the user is. If you have time, try to use CSS transitions to animate it so the bar goes from 0-1 on the first page, 1-2 on the second page and so on (with a smooth and nice animation).


Direct links to wireframes:

[Step 1a](https://github.com/HackYourFuture-CPH/HTML-CSS/blob/master/Week3/wireframes/Step%201a.pdf)

[Step 2](https://github.com/HackYourFuture-CPH/HTML-CSS/blob/master/Week3/wireframes/Step%202.pdf)

[Step 3](https://github.com/HackYourFuture-CPH/HTML-CSS/blob/master/Week3/wireframes/Step%203.pdf)

[Step 4](https://github.com/HackYourFuture-CPH/HTML-CSS/blob/master/Week3/wireframes/Step%204.pdf)

Below is an overview of the fields in the form and how they should be validated. To figure out the right regular expression pattern try googling for something like ("regex only letters") and use something like [this website](https://regexr.com/) to test that the pattern you have found works correctly.

| Field name                   | Required | Validation criteria                                    |
|------------------------------|----------|--------------------------------------------------------|
| First name                   | yes      |                                                        |
| Last name                    | yes      |                                                        |
| Country                      | yes      |                                                        |
| Street address               | yes      |                                                        |
| Post code                    | yes      | Assume danish address, so allow only 4 letters.        |
| Profile description          | no       | Maximum 500 characters                                 |
| Shipping address             | yes      |                                                        |
| Email                        | yes      | Allow only valid email addresses.                      |
| Phone                        | no       | Allow only valid phone numbers                         |
| Password                     | yes      | Minimum 10 characters, uppercase and lowercase letters |
| Password repeat              | yes      | Minimum 10 characters, uppercase and lowercase letters |
| Newsletter                   | yes      | One radio option must be selected                      |
| Kind of items                | no       | Must be possible to select 0, 1 or many options.       |
| "Resemble your style" images | no       | Must be possible to select 0, 1 or many options.       |
| Name on creditcard           | yes      |                                                        |
| Card type                    | yes      |                                                        |
| Credit card number           | yes      | Only numbers allowed. Exactly 16 digits.               |
| Expiry month                 | yes      |                                                        |
| Expiry year                  | yes      |                                                        |
| CCV                          | yes      | Only numbers. Exactly 3 digits.                        |

## Form validation *optional*
For the forms create sensible form validation. Read up on form validation [here](https://css-tricks.com/form-validation-part-1-constraint-validation-html/)

## Hand in Homework:
- With the `https://github.com/USERNAME/hyf-homework`, find the relevant week number
- Now upload your homework files to the repo. 
- If you forgot how to do that, check it out [here](../Week1/homework.md#hand-in-homework)
- Post your index.html file on your classes slack channel in this format: https://htmlpreview.github.io/?https://github.com/YOUR_ACCOUNT/hyf-homework/blob/master/html-css/week1/index.html

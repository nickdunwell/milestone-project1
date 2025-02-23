
# BUFF GYM -  Testing

Visit the deployed site: 

- - -

## CONTENTS

* [AUTOMATED TESTING](#automated-testing)
  * [W3C Validator](#w3c-validator)
  * [Lighthouse](#lighthouse)
* [MANUAL TESTING](#manual-testing)
  * [Testing User Stories](#testing-user-stories)
  * [Full Testing](#full-testing)

Testing was ongoing throughout the build. I utilised Chrome developer tools whilst building to pinpoint and troubleshoot any issues as I went along.

During development I made use of google developer tools to ensure everything was working correctly and to assist with troubleshooting when things were not working as expected.

I utilised the console in the developer tools to work through small sections of JavaScript and ensure that the code was working, and also to troubleshoot where issues were.

I have gone through each page using google chrome developer tools & Firefox inspector tool to ensure that each page is responsive on a variety of different screen sizes and devices.

- - -

## AUTOMATED TESTING

### W3C Validator

[W3C](https://validator.w3.org/) was used to validate the HTML on all pages of the website. It was also used to validate the CSS.

* index.html - [index.html](. When I tried to take it out, the imagery was wrong, so hav eleft them in.
* booking.html - Passed, no errors
* success.html - Passed, no errors.

* style.css - Passed, no errors found.

- - -

### Lighthouse

I used Lighthouse within the Chrome Developer Tools to test the performance, accessibility, best practices and SEO of the website.

### Desktop Results

![lighthouse results](https://github.com/nickdunwell/milestone-project1/blob/main/lighthouse-results.jpg) 
The main performance issues are with image sizing and external font retrieval.
The SEO issues are just because the website has not been deployed amd searchable yet.

### Mobile Results

![index.html](https://github.com/nickdunwell/milestone-project1/blob/main/lighthouse-results-mobile.jpg)
The performance results are, again, because of image sizing and external retrieval.
The SEO issues are the same as desktop.

## MANUAL TESTING

### Testing User Stories

`First Time Visitors`

| Goals | How are they achieved? |
| :--- | :--- |
| I want to see what the gym has to offer | The BUFF GYM homepage has all the information that the user needs, in regards to classes and opening times. |
| I want the site to be responsive to my device. | I have developed the site with responsiveness in mind. |
| I want the site to be easy to navigate. | Buttons are used throughout the site for navigation, much like a mobile app. There is a header, which has all buttons to take to straight to the section the user is interested in. The page logo also acts as a link to the home page.  |
| I want to be able to see members of staff. | There is a section, which shows the various members of staff and which classes they take. |
| I want to be able to find the contact details of the gym | The user can navigate to these by either scrolling down to the footer, or by using the clickable link in the navbar at te head of the page. |

`Returning Visitors`

|  Goals | How are they achieved? |
| :--- | :--- |
| I want to be able to quickly access the section I am interested in. | Users can quickly and easily use the navbar, located in the header of the main page, booking page, or the success page. |

`Frequent Visitors`

| Goals | How are they achieved? |
| :--- | :--- |
| I want to know that everything is where I expect it to be. | The user will find the sections they want will not change over time and, therefore will become familiar. |

- - -

### Full Testing

Full testing was performed on the following devices:

* Laptop:
  * Dell Inspiron 15" screen
* Mobile Devices:
  * iPhone 12.
  

Each device tested the site using the following browsers:

* Google Chrome
* Safari


`Home Page`

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| The Sites logo | Link directs the user back to the home page | Clicked title | Home page reloads | Pass |
| Navbar | Displays Home, Classes, Meet the Team, Contact | Clicked on button | Takes you to the desired section | Pass |
| Book Now button | Directs users to the booking form | Clicked on button | Opens the booking page | Pass |
| 2nd Book Now button | Directs user to the booking form | Clicked on button | Booking page opens | Pass |

`Game Page - Difficulty Selection`

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| The Sites title | Link directs the user back to the home page | Clicked title | Directed back to home page | Pass |
| All buttons - hover effect | All buttons with a black background & white text should change when hovered over to a background colour of white with black text. | Hover over each button on the page | Each button displayed the correct styling when hovered over | Pass |
| 🍺 Cursor | The 🍺 should display when a user moves the mouse over a button | Moved the mouse over each button to check the cursor changed upon entering the button | The cursor changed from the arrow cursor to the 🍺 cursor | Pass |
| Easy Button | Calls the easy quiz URL for the API | By console logging the data called from the API I was able to check the difficulty level of the questions corresponded with the level called | ![data-console.log-easy](testing/data-consolelog-easy.png) | Pass |
| Medium Button | Calls the medium quiz URL for the API | By console logging the data called from the API I was able to check the difficulty level of the questions corresponded with the level called | ![data-console.log-medium](testing/data-consolelog-medium.png) | Pass |
| Hard Button | Calls the hard quiz URL for the API | By console logging the data called from the API I was able to check the difficulty level of the questions corresponded with the level called | ![data-console.log-hard](testing/data-consolelog-hard.png) | Pass |

`Game Page - Quiz Area`

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| The Sites title | Link directs the user back to the home page | Clicked title | directed back to home page | Pass |
| All buttons - hover effect | All buttons with a black background & white text should change when hovered over to a background colour of white with black text. | Hover over each button on the page | Each button displayed the correct styling when hovered over | Pass |
| 🍺 Cursor | The 🍺 should display when a user moves the mouse over a button | Moved the mouse over each button to check the cursor changed upon entering the button | The cursor changed from the arrow cursor to the 🍺 cursor | Pass |
| Question populated | The question from the API is correctly pulled from the JSON data | console.log the data and check that the question has been pulled correctly | The question is displaying | Pass |
| Answers populated | The answers from the API are correctly pulled from the JSON data | console.log the data and check that the answers have been pulled correctly | The answers are displaying | Pass |
| Data attribute correct | The data attribute correct has been applied to the correct answer | By console logging the data I am able to check what the correct answer should be. I can then console.log the id of the buttons to check whether the data attribute has been applied only to the button containing the correct answer | only the correct answer has the correct attribute | Pass |
| Correct answer - border colour | When a correct answer is clicked the border around the game area should display green | Clicked on a correct answer | Border displayed green | Pass |
| Incorrect answer - border colour | When an incorrect answer is clicked the border around the game area should display red | Clicked incorrect answer | Border displayed red | Pass |
| Correct answer - button colour | When a correct answer is clicked the button should change background colour to green | Clicked a correct answer | Button background turned green | Pass |
| Incorrect answer - button colour | When an incorrect answer is clicked the clicked buttons background should turn red | Clicked incorrect answer | Button background turned red | Pass |
| Incorrect answer - display correct answer | When an incorrect answer is clicked, the correct answer should display a green background | Clicked incorrect answer | The correct answer turned green | Pass |
| Question No counter | The Question No counter should start at 1 and increase by 1 time the next button is selected. | answered questions and clicked next button | Each time the next button is clicked the Answer no counter increases by 1. | Pass |
| Score Counter | The score counter should begin at 0. Each time a correct answer is selected the score should increase by 10. If an incorrect answer is selected the score should remain the same | Clicked a correct answer to check if the score increased. Clicked an incorrect answer to check the score stayed the same| When a correct answer was selected the score increased by 10. When an incorrect score was selected the score stayed the same | Pass |
| Not Allowed Cursor | Once an answer has been selected, the answer buttons should then be disabled and when hovered over the not allowed cursor will display | Clicked on one answer button and then clicked on the remaining answer buttons | After the answer was selected each answer button clicked on subsequently displayed the not allowed cursor | Pass |
| Next button - becomes visible | When an answer is clicked the next button should be displayed so the user can progress to the next question, or to the end section if all 15 questions have been answered| Clicked on an answer button | The next button displayed | Pass |
| Next button hover effect | A button with a white background & black text should change to a button with a black background & white text when hovered over.| Hovered over the button | Style changed as expected | Pass |
| Next button - clicked | When clicked all answer styles should be removed, the next button should become hidden again and a new question and answer loaded if there are questions left. If all questions have been answered the end game should appear | Clicked on the next button | All styles were removed and a new question and answers were displayed. After question 15 was answered I was taken to the end game. | Pass |

`Game Page - End of Quiz`

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| The Sites title | Link directs the user back to the home page | Clicked title | Home page reloads | Pass |
| All buttons - hover effect | All buttons with a black background & white text should change when hovered over to a background colour of white with black text. | Hover over each button on the page | Each button displayed the correct styling when hovered over | Pass |
| 🍺 Cursor | The 🍺 should display when a user moves the mouse over a button | Moved the mouse over each button to check the cursor changed upon entering the button | The cursor changed from the arrow cursor to the 🍺 cursor | Pass |
| Score Display | The Your Score area should populate with the score you have achieved | I added my score as I played, checked the score on the last question & compared to the score displayed | The score displays correctly | Pass |
| Submit Button - enabled/disabled | The submit button should be disabled and show the not allowed cursor by default. Once the user types their team name into the input field the button is enabled | I hovered over and clicked the submit button without filling in the team name field. I then added a team name, hovered over and clicked the submit button | Without a team name filled in the cursor displays as not allowed and the button will not submit. Once I filled in a team name the cursor became a 🍺 when hovered over the button and I was able to click and submit the score | Pass |
| Submit button - on submit | Once clicked the submit button will redirect you to the high scores page | Clicked the button with the team name filled in | Redirected to the high scores page | Pass |
| Play again? button | Clicking on this button will return you to the start of the game page where you can select a quiz difficulty level | Clicked on the play again? button | Directed to the beginning of the game to select a difficulty level | Pass |
| Home button | Clicking on this button will take you back to the home page | Clicked the home button | Directed back to the home page | Pass |

`High Scores Page`

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| The Sites title | Link directs the user back to the home page | Clicked title | Home page reloads | Pass |
| All buttons - hover effect | All buttons with a black background & white text should change when hovered over to a background colour of white with black text. | Hover over each button on the page | Each button displayed the correct styling when hovered over | Pass |
| 🍺 Cursor | The 🍺 should display when a user moves the mouse over a button | Moved the mouse over each button to check the cursor changed upon entering the button | The cursor changed from the arrow cursor to the 🍺 cursor | Pass |
| Score Displayed | If your score is in the top ten, your team name and score will be displayed in the high scores area in descending order | Played 11+ games and logged a variety of scores. | Once 10 scores were displayed on the high scores board, only scores that were better than the ones logged would then be added to the board | Pass |
| Play again? button | Takes the user to the beginning of the game page to select a difficulty level | Clicked the button | Taken to the beginning of the game page to select a difficulty level | Pass |
| Home button | Takes the user to the home page | Clicked the button | Taken to the home page | Pass |

`404 Error Page`

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| The Sites title | Link directs the user back to the home page | Clicked title | Home page reloads | Pass |
| All buttons - hover effect | All buttons with a black background & white text should change when hovered over to a background colour of white with black text. | Hover over each button on the page | Each button displayed the correct styling when hovered over | Pass |
| 🍺 Cursor | The 🍺 should display when a user moves the mouse over a button | Moved the mouse over each button to check the cursor changed upon entering the button | The cursor changed from the arrow cursor to the 🍺 cursor | Pass |
| Go home button | Takes the user back to the home page | Clicked the button | Taken to the home page | Pass |
| Play button | Takes the user to the beginning of the game page | Clicked the button | Taken to the beginning of the game page to choose a difficulty level | Pass|
| View high Scores button | Takes the user to the high scores page | Clicked the button | Taken to the high scores page | Pass |

`500 Error Page`

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| The Sites title | Link directs the user back to the home page | Clicked title | Home page reloads | Pass |
| All buttons - hover effect | All buttons with a black background & white text should change when hovered over to a background colour of white with black text. | Hover over each button on the page | Each button displayed the correct styling when hovered over | Pass |
| 🍺 Cursor | The 🍺 should display when a user moves the mouse over a button | Moved the mouse over each button to check the cursor changed upon entering the button | The cursor changed from the arrow cursor to the 🍺 cursor | Pass |
| Go home button | Takes the user back to the home page | Clicked the button | Taken to the home page | Pass |
| View high Scores button | Takes the user to the high scores page | Clicked the button | Taken to the high scores page | Pass |

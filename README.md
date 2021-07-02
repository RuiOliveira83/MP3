# [The Sweet Project](https://ruioliveira83.github.io/MP3)
![Responsiveness](readme-images/amiresponsive.png)
The main purpose of this project is to create a full-stack website where the community can share and search dessert recipes in a easy to navigate and clean looking website, using HTML, CSS, JavaScript, Python, Flask and MongoDB.
This website is my third milestone project for the diploma in software development from the [code institute](https://codeinstitute.net). 
A live view of this website can be found here: [The Sweet Project](https://sweet-recipes-project.herokuapp.com/).

---
## UX

### User Stories
* As a regular user, I want a website responsive and good looking on all devices;
* As a regular user, I want a website easy to navigate;
* As a regular user, I want to see and get inspired by dessert recipes;
* As a regular user, I want to be able to search recipes;
* As a regular user, I want to see all the recipes in each category;
* As a registered user, I want to have all the funcionalities of a regular user and some extra functionalities;
* As a registered user, I want to make use of CRUD (create, read, update and delete) for my recipes;
* As a registered user, I want to quickly see all my recipes;
* As a Admin user, I want to have all the funcionalities of a registered user and some extra functionalities;
* As a Admin member, I want to be to make use of CRUD (create, read, update and delete) for all recipes; 
* As a Admin member, I want to be to make use of CRUD (create, read, update and delete) for the categories; 


### Wireframes
It was used [Balsamiq](https://balsamiq.com/) to create the following wireframes:
| Desktop                                                        | Tablet and Mobile                                             |
| -------------------------------------------------------------- | ------------------------------------------------------------- |
| [Home](wireframes/desktop-home.png)                            | [Home](wireframes/mobile-home.png)                            |
| [Register](wireframes/desktop-register.png)                    | [Register](wireframes/mobile-register.png)                    |
| [Log in](wireframes/desktop-log-in.png)                        | [Log in](wireframes/mobile-log-in.png)                        |
| [Add Recipe](wireframes/desktop-add-recipe.png)                | [Add Recipe](wireframes/mobile-add-recipe.png)                |
| [Edit Recipe](wireframes/desktop-edit-recipe.png)              | [Edit Recipe](wireframes/mobile-edit-recipe.png)              |
| [Manage Categories](wireframes/desktop-manage-categories.png)  | [Manage Categories](wireframes/mobile-manage-categories.png)  |
| [User Page](wireframes/desktop-user-page.png)                  | [User Page](wireframes/mobile-user-page.png)                  |

---
## Features
### Existing Features
The users of this website can be divided in 3 categories: **Unregistered user**, **Registered user** and **Admin**.
All pages of this website share the same footer, this footer allows the user to go to the social media pages of this brand.

The **Unregistered users** can see and search all the recipes and can filter the recipes by category.
On the unregistered users' header there are 4 options:
- return home and see all the recipes;
- filter the recipes by categories and see all the recipes for each category;
- log in, if the unregistered user has an account and want to enter the account;
- register, if the unregistered user wants to create an account and become a registered user.

The **registered users** can see and search all the recipes and can filter the recipes by category.
**Registered users** can add new recipes.
**Registered users** can edit and delete the recipes added by them.
On the registered users' header there are 5 options:
- return home and see all the recipes;
- filter the recipes by categories and see all the recipes for each category;
- go to the user's page, to see all the recipes added by the user;
- add new recipes;
- log out.

The **Admin users** can see and search all the recipes and can filter the recipes by category.
**Admin users** can add new recipes.
**Admin users** can edit and delete all the recipes.
**Admin users** can add new categories and delete categories.
The admin users' header is similar to the registered users header, but has a extra option to manage categories.

The **Home** page has a section with a search bar, where the user can search for a recipe.
Below the search bar there are up to 8 cards with recipes. There is a limit of 8 recipes per page, if the user wants to see more recipes, the user needs to go to the next page. Each card has the option of opening the recipe page, and the option to edit or delete the recipe, if the recipe was added by the user, or if the user is an admin user.

The **My_recipes** page shows cards with the recipes added by the user. Each card has tree options:
- View recipe;
- Delete Recipe;
- Edit Recipe.
The my_recipes page is paginated and there is a limit of 8 cards per page.

The **Recipe** page has:
- the recipe name;
- a recipe picture (if a picture wasn't added when the recipe was added a generic picture will be shown);
- A list with the recipe categories. The displayed categories have a link to all the recipes with the same category;
- A recipe description;
- The recipe ingredients;
- The recipe method;
- If the recipe was added by the user there will be 2 buttons on the bottom that allow the user to edit or to delete the recipe.

The **Add Recipe** page has a form where the user can add:
- Recipe's name;
- Recipe's description;
- Recipe's Categories;
- Recipe's Ingredients;
- Recipe's Method;
- Recipe image's URL.
On the bottom of the page there is a button to add the recipe to the database.

The **Edit Recipe** page has the same form as in the edit recipe, but the form is pre filled with the information to be edited.
On the bottom of the page there are two buttons:
- one edit button that will save the changes, edit the recipe and return to the user's my_recipe page;
- one cancel button that will return the user to the home page without saving the changes.

The **Register** page has a

It was used defensive programming on the delete function (both delete recipe and delete category). A category or a recipe can't be deleted with just one click, the user needs to confirm that he really wants to delete the item, to avoid unintencional actions from the user.

---
## Technologies Used

### Languages Used
- [HTML5](https://en.wikipedia.org/wiki/HTML5)
  - The programming language used to provide content and structure.
- [CSS3](https://en.wikipedia.org/wiki/CSS)
  - The programming language used to format the styling.
- [JavaScript](https://en.wikipedia.org/wiki/JavaScript)
  - The programming language used to make the web page interactive.
- [Python (including Jinja)](https://www.python.org/)
  - The programming language used to build the backend functionality.
### Frameworks and Libraries Used
- [Gitpod](https://gitpod.io/)
  - IDE (Integrated Development Environment) used to develop this project.
- [GitHub](https://github.com/)
  - The code hosting platform used to host the project.
- [Heroku](https://dashboard.heroku.com/)
  - Cloud platform used to deploy the website.
- [MongoDB](https://www.mongodb.com/)
  - Fully managed cloud database service used to store all the data for this project.
- [Flask](https://flask.palletsprojects.com/)
  -  Web framework used to provide libraries, tools and technologies for this project.
- [Werkzeug](https://werkzeug.palletsprojects.com/)
  - Comprehensive WSGI web application library used for password hashing, authentication and authorization.
- [Balsamiq](https://balsamiq.com/)
  - The software used to create the project's wireframes.
- [Materialize](https://materializecss.com/)
  - In-built JavaScript package for interactive and responsive web-design.
- [Google Fonts ](https://fonts.google.com/)
  - Font families library used to provide the font "Baloo Tammudu 2" and "lobster".
- [jQuery](https://en.wikipedia.org/wiki/JQuery)
  - JavaScript library used to simplify the JavaScript code.
- [W3C Markup Validator](https://validator.w3.org/)
  - The markup validation service used to check for errors in the HTML code.
- [Jigsaw](https://jigsaw.w3.org/css-validator)
  - The CSS validation service used to check for errors in the CSS code.
- [JSHint](https://jshint.com/)
  - The JavaScript validation service used to check for errors in the JavaScript code.
- [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools)
  - Chrome DevTools used to test the responsiveness of the site.
- [Responsive Design Checker](https://www.responsivedesignchecker.com/)
  - Responsive Design Checker used to test the responsiveness of the site.

---
## Testing
### Code Validators
- [HTML Validator](https://validator.w3.org/#validate_by_input) (via direct input path):
  - Home (index.html) - No errors or warnings:
  ![Home Page HTML Validator](readme-images/val-html-index.png)
  - Game (game.html) - No errors or warnings:
  ![Portfolio Page HTML Validator](readme-images/val-html-game.png)
  
- [CSS Validator](https://jigsaw.w3.org/css-validator/#validate_by_input) (via direct input path):
  - No errors found:
![CSS validator](readme-images/val-css.png)

- [JavaScript Validator](https://jshint.com/):
  - No errors found:
![JavaScript validator](readme-images/val-js.png)

### Responsiveness of the website
It was used [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools) and
[Responsive Design Checker](https://www.responsivedesignchecker.com/)
 to test the responsiveness of the site.

![Responsiveness](readme-images/responsiveness.png)

The website structure adapts well to all used screen size.

### Functionality of the website
The responsiveness of all pages was tested:
- the Game Name on the top left corner returns you to the home page;
- the "Tell me what you think" modal is working and, when clicked, a working message box is shown;
- the "How to Play" modal is working and, when clicked, shows the game's rules;
- the buttons to select the game mode are working properly;
- the timer starts when the player starts to play the game;
- the score is working properly: increases the score for every correct answer and decreases the score for every wrong answer. It also starts at 0 points when the player starts a new game;
- the top score is working properly, it keeps the higher score when the player starts a new game;
- the words randomly selected are showing properly.

### Browser compatibility
The appearance and responsiveness of the website was tested with good results in 4 different web browsers: Microsoft Edge,
Mozilla Firefox, Google Chrome and Opera. This website is not compatible with Internet Explorer because it uses promises that are not supported by IE.

### Testing User Stories
* As a regular user, I want a website responsive and good looking on all devices;
  - A regular user will find a website with a balanced design and a clear structure in whatever device he chooses to use.
* As a regular user, I want a website easy to navigate;
  - A regular user will find a website with a clear structure making it easy to navigate.
* As a regular user, I want to be able to start playing the game quickly;
  - A regular user can start playing with just one click, the user just has to select the game mode.
* As a user, I want to be able to read the game rules, if needed;
  - A modal with the game rules is present on both pages and can be accessed anytime.
* As a user, I want to see my score;
  - The score is present on the game page and can be seen anytime.
* As a user I want to be able to see my top score;
  - The top score is shown above the score and can be seen anytime.
* As a user, I want to be able to contact the developer to give my opinion or suggestion;
  - A modal with a contact form is present on both pages.
* As a user I want to play a funny game;
  - The sound for correct or wrong answers make the game more fun, and the challenge of beating one's score makes the game funny and appealing.
* As a user I want to repeat the experience and play again.
  - When the game ends there is an option to play again. The game duration is only 30 seconds to make it more inviting to play "just one more" game.

## Deployment
To __deploy__ the project in GitHub I perform the following steps:
- Log into my [GitHub](https://github.com/) account;
- Choose the project "MP2_Translation-Game" on the Repositories;
- Click on Settings;
- Scroll down to the "GitHub Pages" section;
- Inside the "GitHub Pages" section, click on the drop-down menu under Source and select Master Branch;
- The page refreshes automatically and the website is now deployed.
- The link to the webpage can be found in the GitHub Pages section.

To run the code locally by __cloning__ the project from GitHub:
- Log into my [GitHub](https://github.com/) account;
- Choose the project "MP1" on the Repositories;
- Inside the Code button copy the URL link inside the Clone section;
- Open repository or create a new repository;
- Open terminal;
- Type *git clone* followed by the copied URL and press Enter.

---
## Credits
### Content
- Home Page:

- Overall structure:
  - I've looked at several projects on the code institute slack channel and, even though I didn't use any specific one as direct inspiration,
  it was helpful to see other creators ideas to help form my concept.
- Read me file:
  - I used the code institute template and followed my previous project as a guideline.

### Media
- The image used in the background was taken from [kissclipart](https://www.kissclipart.com/).
- The flags' images used in the game modes were taken from the [iconfinder](https://www.iconfinder.com/)
- The sound effects used in this website were taken from https://mixkit.co/

### Acknowledgements
- The [code institute](https://codeinstitute.net) for the inspiration and knowledge to do this website.
- The code institute [Slack](https://slack.com/) channel, for having an extensive library of questions and answer with almost all my questions.
- My mentor [Precious Ijege](https://www.linkedin.com/in/precious-ijege-908a00168/?originalSubdomain=ng) for guidance and support.
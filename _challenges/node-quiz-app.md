---
title: Node Quiz on Terminal
layout: page
---

# An interactive quiz game built with Nodejs and Open Trivia DB

> Written by: Lan Dang (github.com/hl271)

  

### What you'll get out of this app :)

- Nodejs skills

- Get to know more npm packages (`fs`, `inquirer`)

- Get to know API && how to use an exsisting API (`Open Trivia DB`) to develop app

  

## A. Where to code your Nodejs app

- Code offline (VSCode):

    - How to setup: [Build Node.js Apps with Visual Studio Code](https://code.visualstudio.com/docs/nodejs/nodejs-tutorial)

    -  **Deploy**: Deploy your code to github (\[guide below\](#github)) and send the link to me

- Code online (RePL):

    - Link:  [Repl.it - Online Nodejs Editor and IDE - Fast, Powerful, Free](https://repl.it/languages/javascript)

    -  **Deploy**: After sign up and finish your app, share it to me

  
## B. Description

This quiz game has 3 essential features (`initGame()`, `playGame()`, `saveGameToFile()`):

  

-  **Feature 1: Get input from user when the game start (initGame)**

    - Use `Inquirer` to interactively get the specified informations from user when the game starts: `[username, numberOfQuestion, timePerQuestion, quizCategory]`

    - Use `numberOfQuestion` and `quizCategory` (provided by user) to get quizzes from API \[Open Trivia DB\](https://opentdb.com/api_config.php)

    - Use `username` to greet user

    - Assign `timePerQuestion` to a variable to use later in the game

  

-  **Feature 2: Play game**

    - The game has `n` rounds (`n` is the `numberOfQuestions` that user provides)

    - In each round:

    - Print in the terminal the quiz's description and all possible answers

    - Prompt answer from user and validate its accuracy

    - If the answer is correct, user gets +1 point

    - Else, user gets 0 point

    - Game ended when all of the questions is played

  

-  **Feature 3: Save game to file (OPTIONAL)**

    -  **Hint**: Use the `fs` module

    - Save result of each game to file as a json object, for example:

    ```json

    {

    "username": "Lan Dang",

    "numberOfQuestions": "10",

    "quizCategory": "Science",

    "timePerQuestion" : "5000",

    "totalScore": "8"

    }

    ```

  

## C. Resources

### 1. Neccessary modules

- npm packages required:

    -  `inquirer` - command line utility

    -  `fs (default module, don't need to install)` - write and read file from system

- API:

    -  `Open Trivia DB` - place to get all the questions

- Useful functions:

    -  `fetch(url)` - fetch data from api

  

### 2. Documents and extra resources

-  `Inquirer` document: [GitHub - SBoudrias/Inquirer.js: A collection of common interactive command line user interfaces.](https://github.com/SBoudrias/Inquirer.js/)

  

-  `Open Trivia` document: [Open Trivia DB: Free to use, user-contributed trivia question database.](https://opentdb.com/api_config.php)

  

-  `fs (fileSystem)` module: [Module FS trong NodeJS](https://freetuts.net/module-fs-trong-nodejs-674.html)

  

- Github guide (how to deploy your code) <span  id="github"></span>: [An Intro to Git and GitHub for Beginners (Tutorial)](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)

  

- How to use fetch to get data from an api: [How to Use the JavaScript Fetch API to Get Data ― Scotch.io](https://scotch.io/tutorials/how-to-use-the-javascript-fetch-api-to-get-data)

  

- Understand what an api is: [What is an API? In English, please. – freeCodeCamp.org](https://medium.freecodecamp.org/what-is-an-api-in-english-please-b880a3214a82)

- Nodejs tutorial on W3Schools: [Node.js Tutorial](https://www.w3schools.com/nodejs/)


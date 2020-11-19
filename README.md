# Unit 14 Sequelize Homework: Reverse Engineering Code

Reverse engineer the starter code provided and create a tutorial for the code.

In the `Develop` folder, there is starter code for a project. Begin inspecting the code to get an understanding of each file's responsibility. Then, in a Google Doc, write a tutorial explaining *every* file and its purpose. If one file is dependant on other files, be sure to let the user know.

At the end of the tutorial, add instructions for how you could now add changes to this project.

Following the [common templates for user stories](https://en.wikipedia.org/wiki/User_story#Common_templates), we can frame this challenge as follows:

```
AS A developer

I WANT a walk-through of the codebase

SO THAT I can use it as a starting point for a new project
```

## Business Context

When joining a new team, you will be expected to inspect a lot of code that you have never seen before. Rather than having a team member explain every line for you, you will dissect the code by yourself, saving any questions for a member of your team.

## Acceptance Criteria

```md
GIVEN a Node.js application using Sequelize and Passport
WHEN I follow the walkthrough
THEN I understand the codebase
```
A link to a Google Doc or video explaining the application in `Develop/`. 

_Note: Don't forget to change the sharing settings on your Google Doc._

1) Config:
A) Middleware:
Middleware is software that lies between an operating system and the applications running on it. It enables communication and data management for distributed applications. 
The middleware used in this application is makes sure is a user is not registered that they cant sign in. 
B)Config.json
Contains the data that links the MySQL database to the application.
C)Passport.js
lets the application know that a user must sign in or sign up with a username and password and that you must have one to either login or signup.

2) Models
A) index.js contains data that allows models to communicate with database/config
B) user.js contains the info for generating a database table in MySQL and also require bcyrpt to password hashing.

3) Public
A) CSS contains styles.css for all frontend page styling 
B) JS contains all individual JS functionality indivdual JS Pages 
C) .html contals all indivdual HTML pages for Login page, Sign Up page, and Main landing members page

4) Routes
A) api-routes.js which contain the Get/Post Destroy  Methods along with sequlize ORM to Create Read Update Delete content. In this case just the get and post methods for login and signup.
B) html-routes.js contains the static routing to "/" ,"/login", and "/members" pages which directs you to the page if you are logged in. It also requires the middleware which make sure that you cant access the pages unless you are logged in

5) .gitignore is the files which contains a pattern for files/directories to ignore b/c of data contraints.

6) README.md contains readme file with instructions for application use.

7) package.json and package-lock.json contain file dependencies / libraries we use in the application metadata relevant to the project and it is used for managing the project's dependencies, scripts, versions and much more.

8) server.js contains the info which communicates with the server and allows the user to run the application on a localhostserver.

A link to a Google Doc
https://docs.google.com/document/d/1ePJGucHhLSKYIXT4JPAjtKNgQbaJhNtRBRZvmHr_iEE/

/Develop
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

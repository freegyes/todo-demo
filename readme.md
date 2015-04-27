````
meteor create abf-todo
cd abf-todo
meteor
````

http://localhost:3000/

###STEP01

````
git init
git remote add origin https://github.com/freegyes/todo-demo.git
git fetch origin 01:01
git checkout -f 01
````

- parsing, compiling
    - html head, body, templates
    - js isClient, isServer, smart folders
    - css
    - forced lint & minify

###STEP02

````
git fetch origin 02:02
git checkout -f 02
````

- mongodb & minimongo

````
meteor mongo
db.tasks.insert({ text: "Hello world!", createdAt: new Date() });
````

or in browser console (split screen to show hot code push)

````
Tasks.insert({text: "This is a todo item"})
````

- collections
    + publish & subscribe
    + autopublish & insecure packages 

###STEP03

````
git fetch origin 03:03
git checkout -f 03
````

  - add a form to the html for input
  - handle the submit event in the js
  - sort by creation desc

###STEP04

````
git fetch origin 04:04
git checkout -f 04
````

  - replace template for items
      + {{#each}} {{#if}} {{else}}
  - event handlers in the js (template specific)
  - collection
      + insert, update, remove

<kbd>CTRL</kbd>+<kbd>C</kbd>

````
meteor deploy abf-todo
````

http://abf-todo.meteor.com

````
meteor install-sdk ios
meteor add-platform ios
meteor run ios
````

###STEP05

````
git fetch origin 05:05
git checkout -f 05
````

  - implement hide completed feature
  - Session for storing client related settings
  - auto updating the template & rerun functions
  - add incomplete counter 

###STEP06

````
git fetch origin 06:06
git checkout -f 06
````

add user accounts:

````
meteor add accounts-ui accounts-password

--> {{> loginButtons}}

Accounts.ui.config({
  passwordSignupFields: "USERNAME_ONLY"
});
````

  - http://atmospherejs.com
  - accounts-facebook
  - fontawesome
  - less bootstrap (https://atmospherejs.com/nemo64/bootstrap)

  - show input field only for logged in users
  - save owner on insert
  - show created by username span

###STEP07

  ````
  git fetch origin 07:07
  git checkout -f 07
  ````

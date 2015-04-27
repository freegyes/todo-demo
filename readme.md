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

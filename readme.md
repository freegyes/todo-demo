````
meteor create abf-todo
cd abf-todo
meteor
````

http://localhost:3000/

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


# json-server-todos

Exemple how to create todos api in 30 seconds with json-server

# Installation

```bash
git clone git@github.com:acacha/json-server-todos.git
cd json-server-todos
npm install -g json-server
json-server db_todos.json
```

Now opens:

- http://localhost:3000

You now have a full REST API. Test GET with httpie (or POSTMAN or any other REST Client):

Retrieve all (GET):

```bash
http http://localhost:3000/todos
```

Retrieve one (GET):

```bash
http http://localhost:3000/todos/1
```

Post a task/todo (POST):
 
```bash
http POST http://localhost:3000/todos name="See game of Thrones" done=false priority=3
```

Update Task (PUT):

```bash
http PUT http://localhost:3000/todos/3 name="Fit myself" done=true priority=2
```

Delete task (DELETE):

```bash
http DELETE http://localhost:3000/todos/1
```


# Links

- https://httpie.org/
- https://github.com/typicode/json-server
- Jswon view Chrome plugin: https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc
- Acacha docs: http://acacha.org/mediawiki/Json-server
# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
A backend allows us to persistently store and interact with data used by our application
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The Model
```

Which layer in the MVC pattern communicates with the model?

```bash
The Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Because instead of loading the view from the back end, we choose to load the application view state from our front end client.
```

What does C.R.U.D stand for?

```bash
Create Read Update Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
The Controller
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
index, show, create, update, destroy
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
- client sends get request to the router
- router sees get with a person/:id and tells the person controller to find the show request
- person controller finds the show definition, and executes the request and passes the data along to the person Model
- the model communicates with the backend to retrieve the data requested for the person with id=1
```

What is the command to generate a new rails-api app?

```bash
rails-api new
```

What is the command to start an instance of a rails server?

```bash
rails s
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
-rake db:drop
-rake db:create
-rake db:migrate
```

What is the command to scaffold a pet with a name and an age?

```bash
rails generate scaffold Pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
- They make it easier to test and read our data
- They make your data more secure
```

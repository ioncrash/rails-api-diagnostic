# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
A backend stores data and responds to user requests for access/manipulation
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The controller activates the model, which fetches data from the database
```

Which layer in the MVC pattern communicates with the model?

```bash
The controller communicates with the model to make requests and pass responses back to the router
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
they''re outdated in our version of rails
```

What does C.R.U.D stand for?

```bash
Create Read Update Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
In the model
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```bash
Index, show, create, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
<ol>
  <li>the router determines which controller should handle this action</li>
  <li>the controller passes the request to the model</li>
  <li>the model processes the request, and gets the info from the database, then passes it back to the controller</li>
  <li>the controller passes this info back to the client</li>
```

What is the command to generate a new rails-api app?

```bash
bundle exec rake db:drop db:create db:migrate
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
```

What are the commands to drop, create and migrate a database from the command
line? (3 bullet points)

```bash
db:drop, db:create, db:migrate
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bundle exec rails generate scaffold Pet name:string age:integer
```

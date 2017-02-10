# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
A backend allows a server to access databases and respond to client requests.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
The model.
```

Which layer in the MVC pattern communicates with the model?

```md
The controller.
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Because a view is simply the data that gets sent to the client as a response.
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
The model, because it directly interacts with the database.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
index, create, show, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
- The request goes through the router to the controller
- The controller prepares the commands for the model and then communicates with the model
- The model performs the required actions on the database and sends the data back to the controller
- The controller formats the response and sends it to the client
```

What is the command to generate a new rails-api app?

```bash
bin/rails generate scaffold
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
-bin/rake db:drop
-bin/rake db:create
-bin/rake db:migrate
-bin/rake db:seed
-bin/rake db:examples

```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold Pet name:string age:integer
```

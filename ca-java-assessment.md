## Assessment:
Create a simple Java RESTful application that manages users and tasks for those users.

#### Requirements:
* You do NOT need to create a UI for this application - only REST endpoints.
* The application should be able to list/create/update users via REST.
* The application should be able to list/create/update/delete tasks for users via REST.
* Data must be persisted to a relational database (In-Memory database is acceptable).
* You can use Frameworks(Spring Framework, Java EE etc.) Libraries etc.

#### Considerations:

* Consider usage of a tool/library to manage database schema changes
* Consider containerization of the application
* Treat the code as if it was going to be sent to production - what would you do to ensure it is production-ready.

#### Assumptions:
* Assume that the database will have a high number of tasks and users.
* Feel free to share other assumptions you made during development.

#### Bonus Tasks:  
Setup a scheduled job to check all tasks in the Database - those that have a status of "pending" and who date_time 
has passed - print it to the console
and update the task to "done".

#### Distribution:
Once you are done, please upload the application to a repository and give us access so that we can download/view/test it.
Consider how you would setup this repository if a team of developers is going to working on it.

#### Delivery  
Provide us with a link to an online source code repository after completion.

#### Evaluation Criteria:
We should be able to clone the repo / download artifacts and run it without any installation or configuration.

As a guide, below are the curl commands with the REST endpoints we are expecting to test against.  You can use these urls as a guildeline on how to design/develop your REST endpoints.  

If you do not have access to curl, you can use the Postman client(https://github.com/Competitive-Capabilities-International/client-applications-assessments/blob/master/Java-Assessment.postman_collection.json) (or any other HTTP client) to perform these 
calls in 
order to test your application.

---

#### Create user
```sh
curl --location --request POST 'http://localhost:8080/api/users' \
--header 'Content-Type: application/json' \
--data-raw '{
    "username": "jsmith",
    "firstName": "John",
    "lastName": "Smith"
}'
```

#### Update user
```sh
curl --location --request PUT 'http://localhost:8080/api/users/{id}' \
--header 'Content-Type: application/json' \
--data-raw '{
    "firstName": "John",
    "lastName": "Doe"
}'
```

#### List all users
```sh
curl --location --request GET 'http://localhost:8080/api/users'
```

#### Get User info
```sh
curl --location --request GET 'http://localhost:8080/api/users/{id}'
```
Expecting this structure (for the User):
```
{ 
  "id": 1,
  "username": "jsmith",
  "firstName": "James",
  "lastName": "Smith"
}
```

#### Create Task
```sh
curl --location --request POST 'http://localhost:8080/api/users/{id}/tasks' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name": "My task",
    "description": "Description of task",
    "date_time": "2016-05-25 14:25:00"
}'
```

#### Update Task
```sh
curl --location --request PUT 'http://localhost:8080/api/users/{user_id}/tasks/{task_id}' \
--header 'Content-Type: application/json' \
--data-raw '{"name":"My updated task"}'
```

#### Delete Task
```sh
curl --location --request DELETE 'http://localhost:8080/api/users/{user_id}/tasks/{task_id}'
```

#### Get Task Info
```sh
curl --location --request GET 'http://localhost:8080/api/users/{user_id}/tasks/{task_id}'
```

#### List all tasks for a user

```sh
curl --location --request GET 'http://localhost:8080/api/users/{user_id}/tasks'
```

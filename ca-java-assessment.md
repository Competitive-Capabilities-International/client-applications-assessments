## Assessment:
Create a simple Java RESTful application that manages users and tasks for those users.

#### Requirements:
* You do NOT need to create a UI for this application - only REST endpoints.
* The application should be able to list/create/update users via REST.
* The application should be able to list/create/update/delete tasks for users via REST.
* Data must be persisted to an In-Memory database
* You can use Frameworks(Spring Framework, Java EE etc.) Libraries etc.
* Here is the [Postman collection](https://github.com/Competitive-Capabilities-International/client-applications-assessments/blob/master/Java%20Assessment.postman_collection.json)
with the REST endpoints we are expecting to test against. Ensure request bodies sent when testing your api match what is in the collection.
* Setup a scheduled job to run every minute & fetch all tasks where status is "pending" and date time is in the past and update the task status to "done".

#### Considerations:

* Consider usage of a tool/library to manage database schema changes
* Consider containerization of the application
* Treat the code as if it was going to be sent to production - what would you do to ensure it is production-ready.

#### Assumptions:
* Assume that the database will have a high number of tasks and users.
* Feel free to share other assumptions you made during development.


#### Distribution:
Once you are done, please upload the application to a repository and give us access so that we can download/view/test it.
Consider how you would setup this repository if a team of developers is going to working on it.

#### Delivery  
Provide us with a link to an online source code repository after completion.

#### Evaluation Criteria:
We should be able to clone the repo / download artifacts and run it without any installation or configuration.



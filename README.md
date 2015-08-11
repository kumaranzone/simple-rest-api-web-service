# simple-rest-api-web-service
Designing a simple web service using Json and flask
README
=====

This is a restful api web service sample using Json and flask. Rest api can be accessed via curl.

GET method curl
---------------

$ curl -i http://localhost:5000/todo/api/v1.0/tasks


POST method curl
----------------

$ curl -i -H "Content-Type: application/json" -X POST -d '{"title":"Read a book"}' http://localhost:5000/todo/api/v1.0/tasks


PUT method curl
---------------

$ curl -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/todo/api/v1.0/tasks/2


All calls using username & password authentication
---------------------------------------------------

$ curl -u username:password -i http://localhost:5000/todo/api/v1.0/tasks



HTTP Method	URI	Action
----------------------

GET		http://[hostname]/todo/api/v1.0/tasks				Retrieve list of tasks
GET		http://[hostname]/todo/api/v1.0/tasks/[task_id]		Retrieve a task
POST	http://[hostname]/todo/api/v1.0/tasks				Create a new task
PUT		http://[hostname]/todo/api/v1.0/tasks/[task_id]		Update an existing task
DELETE	http://[hostname]/todo/api/v1.0/tasks/[task_id]		Delete a task


# todowoo_api_with_django_rest_framework


todowoo_api is a web application that provides a task list application which can add to task lists, view task lists and update, delete, check important tasks and complete tasks and provide api that can authentication signup and create random token , login with token or create random token , get , post , put, and delete

this how to use curl to get json and use appliation api todowoo

windows user curl

signup curl example :
change user name and password 

curl -X "POST" http://localhost:8000/api/signup -H 'Content-Type:application/json' -d "{"username":"indah","password":"abcd1234"}"

signin curl example :

curl http://127.0.0.1:8000/api/todos -H "Authorization: Token 0fa879910109e063fd0c649272387a832c4b7410"

linux user curl

signup curl example: 

curl -X "POST" http://localhost:8000/api/signup -H 'Content-Type: application/json' -d '{"username":"nick","password":"abcd1234"}'

signin curl example :

curl http://127.0.0.1:8000/api/todos -H 'Authorization: Token 0fa879910109e063fd0c649272387a832c4b7410'

after login user can add/create todo by accessing this url in browser 

http://127.0.0.1:8000/api/todos

for access complate to do list:

http://127.0.0.1:8000/api/todos/completed

for delete to do list : 

http://127.0.0.1:8000/api/todos/1 just change id no 1 with another id to delete

and this how to use complate task todo with curl 

curl -X "PUT" http://localhost:8000/api/todos/1/complete -H 'Content-Type:application/json' -H "Authorization: Token 933888c33a6da2f53683a0dca61a3ea3f9ad02be"

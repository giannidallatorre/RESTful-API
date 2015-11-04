# RESTful-API

Basic RESTful web service using Python with Flask.

### Set up a new virtualenv
    virtualenv flask

### Install the dependencies
    flask/bin/pip install flask
    flask/bin/pip install flask-httpauth

### Run the RESTfull server
    ./flask-TODO

### Example of usage
#### Using curl:

```
# Add new task
curl -i -H "Content-Type: application/json" -X POST -d '{"title":"New task with curl"}' http://localhost:5000/TODO/api/v1.0/tasks
# Upate task
curl -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/TODO/api/v1.0/tasks/2
# Task list with authentication
curl -u admin:changeme -i http://localhost:5000/TODO/api/v1.0/tasks
```

#### Using browser:

[http://localhost:5000/TODO/api/v1.0/tasks](http://localhost:5000/TODO/api/v1.0/tasks)  
[http://localhost:5000/TODO/api/v1.0/tasks/1](http://localhost:5000/TODO/api/v1.0/tasks/1)


### Note:
Authentication with:  
username: `admin`  
password: `changeme`
### References:
[http://blog.miguelgrinberg.com](http://blog.miguelgrinberg.com)

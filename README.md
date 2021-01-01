# Freshworks Assignment 

This project was generated with Node version v14.13.0. Run `npm install` to install all the dependencies.

Perform following action to start:

1.	`npm start` (to start the server)
2.	Open postman for executing create, read and delete a data from a JSON file.

## Create

3. You can create JSON object using the frontend by entering all the details in the given form.

You can set property called time-to-live for a key and write into a json file and this property is an optional. If ttl(in seconds) is given then the key will not be accessed for further read or delete operations after that time duration reached .

												OR

4. You can create JSON object using Postman:-
It should be POST request in this way : Use postman and pass the key value pair in body.
`http://localhost:3000/submit`

{
    "name": "Prakhar Gupta ",
    "age": "22",
    "ttl": "40"
}


## Read

5.	To read all Records, run:
	` GET 'http://localhost:3000/read/all'`

6.	To read a particular record using key, run:

	GET method ( http://localhost:3000/read/key ) 
	eg. http://localhost:3000/read/eOtom8PSxDs1hfv


## Delete

7. To delete all Records, run:
	` GET 'http://localhost:3000/delete/all'`


8.	To delete a particular record using key, run:

	GET method ( http://localhost:3000/delete/key ) 
	eg. http://localhost:3000/delete/eOtom8PSxDs1hfv


### Note: 

For reading and deleting a particular record using key, time to live duration is 120sec(2mins) after that the key will expire. If ttl is not given then it can be accessed everytime!
	1. What is NPM? 
	Node Package Manager

	2. What does CRUD stand for?
	Create Read Update Delete

	3. When adding middleware to and Express Application, where would you need to include the middleware after it's been
    installed?  For example, how would you include the body-parser middleware?
   	At the beginning of the JS file, it should look like:
   		var express= require('express'),
   			bodyParser= require('body-parser')
   	OR:
   		var express = require('express');
   		var bodyParser= require ('body-parser');

	4. What are the four HTTP verbs that we should be using?
	GET, POST, PUT, DELETE

	5. What is the command to list all of my databases in psql?
	\LIST or \dt

	6. What is the command to connect to a specific database?
	\connect "name of database"

	7. What is the command to show all of my tables in a particular database?
	\d

	8. What does RESTful stand for?
	When creating routes they should represent the "REST" acronym for the HTTP verbs.

	9. What are the 7 RESTful routes?
	List, Show, Edit, New, Create,Update, Delete

	10. What does adding salt do?
	Hash's a user's password, encrypt their password so that no-one can see it

	11. What would be the command to create a new model of Person with the attributes of 'name', 'age', 'height', 'origin'
    (assuming that these would all be strings or integers)?
    db.Model.create({
    	name:string,
    	age:integer,
    	height:integer,
    	origin:string
    	})

	12. What is an ORM?
	Object Relation Mapping
	
	13. Why do we include session data when we authenticate a user?  What would happen if we didn't?
	???
	
	14. How would you make a request for all movies with the word 'wedding' using the NPM module REQUEST?
	var query= req.query.q;
	var URL = "http://omdbapi.com?s="+query;
	request(url, function(err,res,body){
		if (!err && res.statusCode===200){
			var jsonData= JSON.parse(body)
			res.render('search', {movies: jsconData.Search})
		}
		})

	15. What is the difference between authentication and authorization?
	Authorization --> is determining the level of access an individual has in a webpage/database.
	Authentication --> is determing whether or not an individual is who they say they are.

***BONUS***
	16. If you have any specific topics that we have gone over for the past four weeks that you would like us to review, 
     please list those here.
	


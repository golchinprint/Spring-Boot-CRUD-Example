open your browser and enjoy the world

![alt text](http://www.tech-ab.net/wp-content/uploads/2015/11/Spring-Logo.png)
.........

Simple CRUD App Example with Spring Boot

Endpoints :

	/hotels  (get)
		#return all hotles objects in DB


	/hotels/id  (get)
		#return hotel(id) object in DB

	/hotels (post)
		#create a new hotel

	/hotels/id  (put)
		#update hotel(id)

	/hotels/id (delete)
		#delete hotel(id)

-------------------------------

	/passengers  (get)
		#return all passengers objects in DB


	/passengers/id  (get)
		#return passenger(id) object in DB

	/passengers (post)
		#create a new passenger

	/passengers/id  (put)
		#update passenger(id)

	/passengers/id (delete)
		#delete passenger(id)

---------------------------------------
	/hotels/getPsg/id  (get)
		#return passenger of hotel(id)

	/hotels/addPsg/id  (post)  --> id: passengerId
		# set passenger(passengerID) for hotel(id)



Example via postman:
	{
	"name" : "milad",
	"description" : "very amazing!!",
	"city" : "tehran",
	"rating" : 56
	}

Example via curl:

	For Example :

		curl -H "Content-Type: application/json" -X POST 
		-d "{"""name""":"""xyz""","""description""":"""d""","""city""":"""mancity""","""rating""" : 1}"  http://localhost:8080/hotels

Build Project with
		mvn clean package
	Then Run it with 
		java -jar -Dspring.profiles.active=test target/spring-boot-rest-example-0.4.0.war

Simple controller with jquery has been applied to serve the data and update view pages...
You can easily improve this project as conventional sites and use larger and more tables!!

note that This is a good bootstrap for whoever not familiar with SpringBoot!!!!


Very Thanks to Mr.Khoobyari 
[spring-boot-rest-example](https://github.com/khoubyari)



 
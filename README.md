##Web Service for AugmentedReality

#####Technologies used:
* Language: Java
* Framework: Struts2
* DB: MongoDB
* Service type: RESTful(Jersey implementation)

_WAR file present in dist folder(for deployment)_

#####Database structure:
* __DB name__: AugReality
* __Collections__: login, devices
* __Description__:
	a. _login_ - Collection holds login credentials(username and password) of users 
	b. _device_ - Collection holds a document for every user. Each document has an array of device details.
	
#####MongoDB setup:
* Install MongoDB
* Default port: 27017
* Run MongoDB instance(mongod.exe)
* Use MongoShell(mongo.exe) or [RoboMongo](http://robomongo.org/) tool
* MongoDB [documentation](http://docs.mongodb.org/manual/)

#####Web Service Methods:
* __getJson()__: Get the "data.json" file containing device details for the given user. __**Type: GET**__
* __postDevice()__: Receive form field values via PUT request and enter a device document in DB collection. __**Type: PUT**__
* __editDevice()__: Receive updated location values and update existing records in DB collection. __**Type: POST**__
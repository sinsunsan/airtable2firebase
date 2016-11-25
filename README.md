# Airtable 2 firebase synchronisation micro-service 

Airtable2Firebase is a node.js  synchronisation script that read Airtable data and save it to firebase in a way that can be easily requested by a front end.

The development is in progress, so be patient or help us to develop it !

## Key features (developement in progress)

* a configuration file that define which airtable tables to import from which base
* a configuration file to define firebase project and credential to use 
* import options 
   * If the record exist in firebase / Does to update data from airtable at reimport ?
   * ...
* The script will use airtable records ids to prevent creating duplicates in firebase 
* the script  will use node js micro service architecture using a starter like https://github.com/ph0bos/express-microservice-starter

## Why Airtable + Firebase

Because airtable is a great ui, user friendly app to enter the data, and start to bootstrap a product without technicall overhead 
Whereas firebase is great for performance and to prevent spending time in common backend functionnality. 

### What is airtable 

Airtable is a mix between spreadheet and a relation database, with user friendlyness as first design objective. 
https://airtable.com/

### Why Airtable API is not enough to serve an app 

Airtable is great as a user friendly CMS like backend.
It has an api but : 
* this api is not purposed to serve apps with lot's of traffi (limited to 5 query / seconds)
* Also the stucture of the data especially the related tables are not very useful to display related information, without performing a new query.
* The query syntax is limited... 
* It is not possible to set access right to limit access to the data. So this authentication part need to be performed by a backend somewhere.

### What is firebase 

Firebase is an PAAS product adding commonly used features like real time database, cloud messaging, authentication.. to prevent developers to lose time reinventing wheel. 
https://firebase.google.com

### Why Firebase is great

### It is simple, a simple json tree 
For exemple the list of users is accessible at 
users
A unique user with id 21 
users/21
.... 

### It has a authentication system attached to the data

Each part of the json tree can be tested for authentication 
This authentication is called "rules" in firebase.

### Changes are visibe in real time

Thanks to a web sockets like technology, changes are "pushed" to the frontend in real time allowing to get changes in real time. Great for messaging, collaborative, meetings apps !




# Airtable 2 firebase conversion 

### What is airtable 

Airtable is a mix between spreadheet, and a relation database, with user friendlyness as first design objective. 
https://airtable.com/

### Why Airtable API is not enough to serve an app 

Airtable is great as a user friendly CMS like backend.
It has an api but this api is not purposed to serve apps with lot's of traffic.
Also the stucture of the data especially the related table are not very useful to display related information 
The query syntax is limited... 
It is not possible to set access right to access the data, so this authentication part need to be performed by a backend somewhere.

### What is firebase 

Firebase is an PAAS product adding commonly used features like real time database, cloud  messaging, authentication.. to prevent developers to lose time reinventing wheel. 
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

Thanks to a web sockets like technology, changes are "pushed" to the frontend  in real time allowing to get changes in real time. Great for messaging, collaborative, meetings apps !



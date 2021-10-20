This program is all about casting vote, collecting the result at the back end.
This uses the k8 cluster for orchesteration,
The web app is a python base application
The result app is a node.js application
The worker is .Net application user to fileter the result of the vote, that is being stored in the temporaly redis db

Flow:
Front end python-app
store in a temporary redis db
filter on the .Net application
stores the casted vote in a permentent databse
Backend application is Node.js
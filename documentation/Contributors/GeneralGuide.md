# General Guide
RPI Machines Map follows a Model, View, Controller design pattern.
The model is the database that contains all the information to be displayed
on the website. 
The view is the HTML website that the user interacts with.
The controller is responsible for communicating between the model and 
the view so that the users get what they want. 

Since the project follows the MVC struture, all the code is divided into 3 types.
All the HTML pages in the project are located in the "public/views" folder.
The database we use is MongoDB. The file server.js in the main folder is 
responsible for requesting information from the database. 
Then all the controllers are located in the "public/controllers" folder. 
The controllers are in charge of receiving and storing the information from 
the server to be accessed by the views later.

More guides for GitHub and making contributions can be found [here](.).
# Modifications

Here is a general guide on how to make the changes you want.

## Machines Info Page
To modify a specific machine information, 
you must make the modifications on MongoDB.
The machine information is pulled from the database, 
so making changes to local files will not change the information on the page.

To make a modification for all the machine page, make the change in 
[rpicampusmap/public/views/machine_sites_info.html](../../public/views/machine_sites_info.html).
Decide where you want to make the modification on the webpage then find the 
spot for it in the html file.__
For example, you can add an extra row in the "Shop Hours" by adding 
"\<p\>Extra Hour\</p\>" right below "\<p\>Saturday\</p\>".

## New Machine Feature
To add a new machine feature, first you must make the changes in the database. 
Modifying the local machine information files will not be sufficient.

After adding the new feature to the database, you have to make it into 
a scope variable in the controller file. 
All the scope variables for machines are located in 
[rpicampusmap/public/controllers/machineInformationController.js](../../public/controllers/machineInfoController.js).
You set your scope variable to the name of the new feature you addded. 
i.e., $scope.newvariable = httpResponse.data[0].contents.newfeature;

Once you add the new feature to a scope, you can access that scope in the html file.__
Since we added the new scope to the machine controller, 
the scope will be available in 
[rpicampusmap/public/views/machine_sites_info.html](../../public/views/machine_sites_info.html)
via "{{newvariable}}"
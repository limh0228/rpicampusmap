# Modifications

Here is a general guide on how to make the changes you want.

## Machines Info Page
To modify a specific machine information, 
you must make the modifications on MongoDB.
The machine information is pulled from the database, 
so making changes to local files will not change the information on the page.

To make a modification for all the machine page, make the change in 
![public/views/machine_sites_info.html](public/views/machine_sites_info.html).
Decide where you want to make the modification on the webpage then find the 
spot for it in the html file. 
For example, you can add an extra row in the "Shop Hours" by adding 
"<p>Extra Hour</p>" right below "<p>Saturday</p>".

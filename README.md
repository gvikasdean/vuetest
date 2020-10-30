# vuetest
Vue Node


Project Upstar

IDE: Visual Studio Code

How to run

Client

1.	Open the terminal in the project folder
2.	Go to the client directory by typing: ‘cd client’
3.	Type the following command in the terminal: ‘npm run serve’ 
4.	At the end of the process, it will tell the server and port on which the project is deployed. As of now it will be running on the localhost.
5.	Open the link. Now it will display the homepage of the website

Server

1.	Type the following command:’node server/index.js’
2.	Now it will start listening on the port 8000 of the localhost.


What has been covered so far

A.	Database used as part of the project: MongoDB

1.       Created a MongoDB database : BoxDB
2.       Created 3 Collections

a.      Items  : This is similar to products. It will store the details of the items such as itemid, name, price, quantity, imageFiles and rating.

b.      Boxtype  : This is used for creating standard Box types for storing predefined items. Along with that, this stores the type, name, free shipping limit and total price.

c.      BoxCart  : This contains the user specific Box carts. 

3.	Used MongoDB API in the server side project to connect to the database. It defined the user name, database name and the password to the remote database.
 
B.  Server Side APIs:

Created APIs in the server side code to receive requests for various operations to be performed on the data. The various requests incorporated are: GET, POST, PUT, DELETE. 
Used ‘app.use’ and routers to route the request to the corresponding method.

Client Side Models:

Created model classes for Items, Box Carts and BoxTypes to define the values for data members and create requests for server side APIs.

C. Admin Panel Functionalities:

1.	Items Maintenance: 

It will display all the items in the Items collection.
Admin can update existing items by changing their price, quantity and name.

2.	Create New Box:
Using this, the admin can create a new box type by filling in box type, box name and its free shipping limit.

3.	Modify Box Type:

This will display the details of the existing box types.
The user can modify the box types by increasing/ decreasing the quantities of the items or deleting them.

4.	Create Box Cart:

This gives provision for creating a box cart from amongst the existing box types.
As a result, the box cart will contain the items that have been predefined in the corresponding box type.

5.	Modify Box Cart:
Using this, the box cart can be modified by deleting items alreading existing in the cart, changing their quantities and adding new items.

D. User functionalities

1.	Loading products/items details on the front end.
2.	Upon clicking the ‘Add to cart’ button, the item is added to the user cart.


Pending

Modify AppHeaders program to reflect the changes in the cart in the AppHeaders.vue file.
Currently, the users and boxtypes on the admin panel have been hard coded. Their dynamicity is yet to be added.
Display list of items in the box cart and images for the user

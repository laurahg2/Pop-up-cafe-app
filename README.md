# Overview

The client has launched a pop-up cafe in a busy business district. They are offering delivered home-made lunches and refreshments to the surrounding offices. As such, they require a software application which helps them to log and track orders.

This was a 6-week, individual project.

#Requirements From Client

I want to maintain a collection of products and couriers.
When a customer makes a new order, I need to create this on the system.
I need to be able to update the status of an order i.e: preparing, out-for-delivery, delivered.
When I exit my app, I need all data to be persisted and not lost.
When I start my app, I need to load all persisted data.
I need to be sure my app has been tested and proven to work well.
The app should handle errors well

#Flow of the App

An example of the what happens when you run the app:

Open the app
The Main Menu shows four options: Press 1 for Product Menu, 2 for Courier Menu, 3 for Order Menu, or 0 to exit
After pressing 1, the options are: Press 1 to display the list of current products, 2 to create a new product, 3 to update a product, 4 to delete a product.
After pressing 1 again, the list of products currently in the CSV/database will be shown. You will be prompted to press 0 to return to the main menu when you've finished looking
Press 0 to return to the Product Menu
Press 0 to return to the Main Menu
Press 0 to close the app

#The Process

Every week, we received a new markdown with tasks/updates to complete. We were learning new content, and then applying what we had learned to the project - this meant that week by week, the tasks gradually became more advanced.
We started with temporary lists of products and couriers in our code to create, read, update and delete products/couriers from list.
We then moved to text files for persistence, so we had to read from and write to external files instead of temporary lists.
Next, we created a temporary dictionary of orders, since the order data were two-dimensional (it included a customer's name, address, phone, courier, status and the items they ordered), unlike the product or courier lists which were one dimensional.
Our next task was to move our products, couriers and orders to CSV files (so we added prices to our products and phone numbers to our couriers to make them two-dimensional). From the CSV files, I loaded the data as dictionaries, rather than lists. This completely changed how I accessed variables, especially when needing to update data from user input. I made new temporary dictionaries in my update functions to add the CSV line numbers as keys, so the user wouldn't have to type out the entire product/courier/order name - they could just put in a number instead.
In week 5 and 6 of this project, our task was to maintain all of our data in a database. We used Docker to set up our local MySQL databases, and used the MySQL commands to create tables, insert into them, and update or delete directly from them.

Capstone 2 Schema

    The database will be seeded with table on insects. It should include
the species, price, and url to the image. I Since there is no login feature,
a users table is not necessary except as a stretch goal. Such a users
table would contain username, password, email, and orders. No associations
between the online store's inventory and users is necessary as all data linking
the two would be collected on the checkout page. When an insect/product
is purchased, an entry in an 'orders' table with the user's info: phone
number, street address, date/time of order submission and items purchased.
If there is a table for users the orders table would have a foreign key 
reference to the user. I'm going to keep the order info seperate from users 
info so that I can have orders without users and when users are implemented
they can have orders with unique contact and delivery details. 

Insects
- id        
- species      
- price
- url_image

Orders
- id
- phone
- delivery_address
- submit_time
- items

(Stretch)
Users
- id
- username
- password
- email
- orders

        1      to     Many
Orders.items --->>> Insects.id

(Stretch)
Users.orders --->>> Orders.id





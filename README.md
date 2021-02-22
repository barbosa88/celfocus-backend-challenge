# Challenge
Implement a RESTful API to manage a shopping cart.

#### API First
At this stage, a swagger file must be created according to the resources and operations described below.

#### API Resources
This API will manage at least 1 resource (carts).  
A cart can be described by the following properties:
- Creation date
- Status
- Items
- Delivery address
- Owner
- Price
- Checksum

An item can be described by the following properties:
- Name
- Description
- Unit price
- Quantity

#### API Operations
This API must support the following operations:
- Retrieve all carts (with filters support);
- Create a cart;
- Update a cart;
- Remove a cart;

#### API Notes
- Every cart expires after 3hours of its creation;
- No operation is allowed after the cart is expired;
- Cart status must not be saved in the database;
- Support 2 types of checksum generator (eg: MD5, Base64). The checksum must be returned within the resource;
- Use the following properties to generate the checksum: Items, delivery address & owner;
- The checksum to use must be defined in the application properties file;
- Please consider the best approach to manage the cart items, for instance: How to remove an item?;


#### Implementation
Use the following technology stack:
- Java 8 (or 11)
- Spring boot
- MongoDB
- Junit/Mockito
- Lombok/Mapstruct (Not mandatory, but appreciated :))
- Maven

We suggest to use <a href="https://start.spring.io/" target="_blank">Spring initializr</a> to generate your project.

#### Delivery Notes
Please fork this repository and send by mail.



# Challenge
Implement a RESTful API to manage a shopping cart, using the technology stack described below. 


## Data Model
This API should manage at least one resource - shopping cart - but others may be created to support the implementation.

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


## Requirements
This API should implement the following operations to manage the Shopping Cart resource:
- Retrieve all carts (with filtering support);
- Create a cart;
- Update a cart;
- Remove a cart;

Managing cart items can be done in different ways, choose the best option which allows you update individual item quantity or remove a specific item from the cart.

Additionally, the api should be able to calculate a checksum of the Shopping Cart:
- Support 2 types of checksum generator (eg: MD5, Base64). The checksum must be returned within the resource;
- Use the following properties to generate the checksum: Items, delivery address & owner;
- The checksum to use must be defined in the application properties file;

Take in consideration that:
- Every cart expires after 3hours of its creation;
- No operation is allowed after the cart is expired;
- Cart status must not be saved in the database;
  

## Technology Stack
The candidate should use the following tools / frameworks to support the implementation of the API:
- Java 8 (or 11)
- Spring boot
- H2 DB
- Junit/Mockito
- Maven
- Lombok/Mapstruct (not mandatory, but appreciated)


We suggest using our minimal setup provided in the template to minimize setup time.  
We expect you to add other relevant dependencies required for your own implementation.  

#### Default configuration 
- Server is running on port 8083
- H2 console is available at http://localhost:8083/h2-console/
- Swagger UI is available at http://localhost:8083/


# Evaluation Criteria
The following points should be taken into consideration by the candidate to make sure the code submitted is readable and in general, easy to analyze by the evaluating team:
- Effective class, method, and variable names  
Names chosen for classes, methods, and variables should effectively convey the purpose and meaning of the named entity;

- Effective top-down decomposition of algorithms  
Avoid code duplication by factoring out common code into separate routines. Routines should be highly cohesive. Each routine should perform a single task or a small number of highly related tasks. Routines that perform multiple tasks should call different subroutines to perform each subtask. Routines should be relatively short in most cases;

- Code layout should be readable and consistent  
The layout of your code should be readable and consistent, giving attention to things like placement of curly braces, code indentation, wrapping of long lines, the layout of parameter lists, and others;

- Effective source tree directory structure  
The source code is organized into subdirectories, making clear the separation of concerns and layers of the application;

- Effective file organization  
Source code is organized into multiple files. Each class is placed in a separate file. Lumping all of your code in one or two files is not acceptable;

- Correct exception handling  
The program handles exceptions correctly, treating any error gracefully;

- Good unit test cases  
The unit test covers all application layers. In this exercise at least java unit tests should be implemented;


# Submission
To submit the code for the exercise, the candidate should clone the repository, as described in the following link https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template. In the step 5 of the instructions, you should make your repo PRIVATE.
After the private repo is created, you must give permissions to the following list of users:
- joserbatista
- barbosa88
- lalmeida78

<b>DO NOT FORK</b> the original repo!

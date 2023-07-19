﻿# wpl-car-sales

## Project Description: 
Our website Car Bazaar is an idea about providing a convenient platform for users to search for and buy used cars in good condition, while paying a lesser price. On our website any new user can browse cars and see their details with high quality images. For this, the user does not require to create an account. But if the user wants to add cars to her wishlist or proceed to buy a car, she will need to create an account with a proper email address and a strong password. 

On the home page, user can search for a car with a title name, or she can use filters like Brand (Make), Body type or Fuel Type. In addition to this she can use sorting by price functionality to order the items low to high or high to low in price. If the user likes a car, she can go to the details page to see high quality images and features etc. 
If the user is logged in with proper credentials, she can save the item on her wish list or if later she decides to buy the car, she can proceed to buy the car after filling in proper payment details, and the item will be listed into her purchase list.

## Assumptions: 

*	Here we are assuming that common users can not add or remove from car listings.
*	They can buy and save car items.
*	The website belongs to a company that is in the car business. And they have only one Admin who manages the listings.


## Database Design:

We are using MongoDB for data storage of cars and users collections. Description and example of each data model is following:

### Users data model:
<img width="360" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/fdbb2e86-70ef-46e9-a9bc-c5da212ad197">

For user we are taking minimal essential requirements, as email(will work as username) and password. favorites and purchases array are filled at runtime as user saves or buys any car.

### Cars data model:
<img width="476" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/9423fbde-cf9a-4812-8f58-2755894682aa">

As seen in the screen show the cars collection stores all the important details related to cars. Additionally, paymentInfo is updated in runtime when car is bought. The isAvailable attribute becomes false at runtime if the car is bought or deleted by manager.

### Payment data model(sub-document of Cars):
<img width="212" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/1a816623-a4fa-4af0-a5ad-f8fba390a38f">

## Tools and Technologies Used:
For implementation of this website following languages and frameworks are used. 
Client-side:




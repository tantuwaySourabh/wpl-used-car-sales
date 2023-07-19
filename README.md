# wpl-car-sales

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
*	React framework
*	Javascript
*	HTML, CSS and Bootstrap

Server Side: 
* Express Framework for NodeJS
* Passport library for local authentication

Database: 
* MongoDB Atlas for hosting collections over cloud.


## Mail Functionality:
Login and Registration: 

<img width="222" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/ac1e03ed-b7cf-4291-8774-5f919b00a027">
<img width="223" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/cb968734-6896-4863-aafc-40839cae8f2f">

Homepage (Browsing, Searching, Filtering and Sorting):

<img width="486" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/6f5a54bc-5446-446e-a3cc-c8e645c85300">

Car details and images:

<img width="485" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/92a1c1fe-9740-44ba-a600-766c83208c90">

Payment details:

<img width="489" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/03dded29-cde0-40b7-b3b1-1909791d6df3">

Wishlist:

<img width="494" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/8f666220-a128-4742-b249-f65af0c6992e">

Purchase History:

<img width="494" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/b3fec42f-95aa-46f3-8360-808d1ece526c">

Edit Item(Admin Page):

<img width="493" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/5ee97489-2538-4644-8f88-58aeb0ae722a">

Add Item(Admin Page):

<img width="490" alt="image" src="https://github.com/tantuwaySourabh/wpl-used-car-sales/assets/26655938/1b872525-9a30-4847-90e0-30f42b274638">



Video Demo Link: https://youtu.be/SQspNbTZzJQ 















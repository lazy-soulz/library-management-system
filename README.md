## library-management-system

This is a library management API Backend for the management of the users and the books

## Routes and the Endpoints 

## /users

GET: get all the list of users in the system
POST: create/Register a new user 

## /user/{id}
GET: Get a user by their ID
PUT: Updating a user by their ID
DELETE: Deleting a user by thier ID (check if the user still has an issue book) && {is there any fine/penalty to be collected}

## /user/subscription-details{id}

GET: Get a user subscrition details by their ID
  >> Date of subscription
  >> Valid till ?
  >> Fine if any ?

## /books 
GET: Get all the books in the system
POST: Add/create a new book to the system

## /book{id}

GET: Get a book by its ID
PUT: Update a book by its ID
DELETE: Delete a book by its ID

## /books/issued

GET: Get all the issued books 

## /books/issued/withFine
GET: Get all issued books with their fine amounts 

## Subscription Types
  >> Basic (3 Months)
  >> Standard (6 Months)
  >> Premium (12 Months)

>> If a user missed the renewal date, then user should be collected with $100
>> If a user misses his subscription, then user is expected to pay $100
>> If a user missed bith renewel & subscription , then the collected amount should be $200

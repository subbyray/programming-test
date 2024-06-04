# Programming Test

## Goal
You are going to design and build a simple e-commerce RESTful API serivce to fit the following requirement. You are free to use any libraries / progamming languages.


## Background
- The e-commerce site's traffic is around 20 active users per minute.
- There is no spike traffic


## User requirements

- User name must be unique
- Each login session will be expired after 7 days
- When a product item is purchased, the quantity will be deduced
- Product item cannot be over purchased (i.e. `quantity` cannot be negative)
- Once an order is compeleted, the user's balance will be deduced by the order amount
- Each user has $100 balance when they sign up, and the user's balance cannot be negative.


## Technical Requirement
- Authorization is required to all endpoints except for the `login` & `signup` endpoint
- Test cases are required
- Design database table(s) to fulfill the requirements, and provide SQL statement for table creation
- Provide an ERD (Entity relationship diagram) 
- User password cannot be stored in plain text
- Provide a setup guidance 
- Source code must be stored in a git repository (github /gitlab / bitbucket)


## Seed data

Seed data are under [assets/backend](assets/backend/) folder. You can import into your preferred database.

## Endpoints Reference

You are going to build the following endpoints. You are free to define the input and output parameters and the URL as well.

### Sign up

User can sign up with user name and password

---

### Login

Use user name and password to log in and get an authorization token

---
### Order items

Order product item(s) and make an order. The operation should be transactional.

---
### Get my order

Show the user's order(s) and a list of items inside the order.

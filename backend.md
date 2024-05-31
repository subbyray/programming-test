# Programming Test


# Question 1

Use the following undirected graph ­- nodes can be visited only once:

![List](assets/web/graph.png)

- a. Write a function that returns all the possible paths between A­-H.
- b. Write a function that returns the shortest path between A­-H.


# Question 2

## Goal
You are going to design and build a simple e-commerce RESTful API serivce to fit the following requirement. You are free to use any libraries / progamming languages.

## Background
- Seed data are under [assets/backend](assets/backend/) folder. You can import into your preferred database.
- Users are already pre-registered in the database. No user creation is needed.
- All users' password are masked by `sha1` and all the actual password are `password123`


## User requirements
- Authorization is required to all endpoints except for the `login` endpoint
- Each login session will be expired after 7 days
- When a product items is purchased, the quantity will be deduced
- Product item cannot be over purchased (i.e. `quantity` cannot be negative)
- Once the order is compeleted, the user's balance will be deduced by the order amount
- User's balance cannot be negative


## Technical Requirement
- Test cases are required
- Using database is required
- You may need to design new database table(s)
- Provide a setup guidance 
- Source code must be stored in a git repository (github /gitlab / bitbucket)
- The code is expected to be `production ready`


---

## Endpoints Reference

You are free to define the input and output parameter.

### Login

URL: `/login`

Description: 

Use `username` and `password` to log in and get an authorization token

---
### Order items

URL: `/order`

Description: 

Order product item(s) and make an order. The operation should be transactional.

---
### Get my order

URL: `/my_order`

Description:

Show the user's order(s) and a list of items inside the order.
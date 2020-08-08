# User Authentication Service

## Table of Contents

- [APIs](#apis)
- [Quick Start](#quick-start)


## APIs

- `POST: /api/v1/users/auth/signup`

  `payload:
{
  "name" : "John",
  "email" : "john@test.com",
  "password" : "qwerty123"
}`

  Add a new user the database.
  
- `POST: /api/v1/users/auth/login`

  `payload:
{
  "email" : "john@test.com",
  "password" : "qwerty123"
}`

  Login to the service and generate a token.

- `GET: /api/v1/users/profile/:id`

  Get the current user information using User ID.

- `PUT: /api/v1/users/profile/:id`

  `payload:
{
  "name" : "John David"
}`

A successful response will be

200: `{ success: true, data: {} }` or `{ success: true, data: [] }`


## Quick Start

- `npm run start` - To start the server.



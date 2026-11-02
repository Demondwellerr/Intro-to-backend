# Intro to Backend – Products CRUD API

A beginner REST API built with Node.js, Express and MongoDB (Mongoose).

## Tech stack
- Node.js
- Express
- MongoDB Atlas + Mongoose
- dotenv, nodemon

## Setup
1. Clone the repo and run `npm install`
2. Create a `.env` file in the project root:
3. Run `npm run dev`
4. The server starts at `http://localhost:3000`

## Product model
| Field | Type | Required |
|---|---|---|
| name | String | Yes |
| quantity | Number | Yes (default 0) |
| price | Number | Yes (default 0) |
| image | String | No |

## API endpoints
| Method | Route | Description |
|---|---|---|
| GET | /api/products | Get all products |
| GET | /api/products/:id | Get one product |
| POST | /api/products | Create a product |
| PUT | /api/products/:id | Update a product |
| DELETE | /api/products/:id | Delete a product |

## Example request body (POST / PUT)
```json
{
  "name": "Pen",
  "quantity": 10,
  "price": 5
}
```

## Project structure
controllers/ request logic
models/ Mongoose schemas
routes/ URL to controller mapping
index.js app entry point
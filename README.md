# Shopping API

This is a simple RESTful API for managing product listings in an online store. This API consist of CRUD Operation

## Features
- **Create** new product listings
- **Read** all or individual product listings
- **Update** existing product listings
- **Delete** product listings

## Endpoints


### git clone 
```bash
https://github.com/parthchilwerwar/gdgc_task_round_backend
````

```bash
npm install
```

### Running on local host 

```bash
node index.js
```

### Get all the Listing 
```bash
curl -X GET http://localhost:3000/listing
```

### GET /listing/:id

```bash
curl -X GET http://localhost:3000/listing/1
```

### PUT POST /listing
```bash
curl -X POST http://localhost:3000/listing \
  -H "Content-Type: application/json" \
  -d '{
    "title": "Dress",
    "description": "A DCute and awesome dress for women",
    "seller": "Girldress",
    "rating": 4.6
  }'
```

### PUT /listing/:id

```bash
curl -X PUT http://localhost:3000/listing/1 \
  -H "Content-Type: application/json" \
  -d '{
    "title": "Updated Smartphone",
    "description": "New model with even better specs.",
    "rating": 4.8
  }'
```

### DELETE /listing/:id

```bash
curl -X DELETE http://localhost:3000/listing/1
```
### Technologies Used
- Express: Web framework for Node.js
- uuid: For generating unique IDs
- Body-parser: Middleware for parsing incoming request bodies
  



State Statistics Management API

A complete RESTful API built using Express.js to manage statistical data of Indian states using an in-memory JSON array.

This project demonstrates:-

REST architecture
GET, POST, PUT, PATCH, DELETE methods
Proper HTTP status codes
PUT vs PATCH difference
Dynamic route handling
Aggregation logic
Resource deletion logic
⚠ No database used
⚠ No authentication
⚠ No validation libraries

🌐 Live Deployment :-

Render Deployment Link:
https://node-assignment-3-1-29zi.onrender.com

📂 GitHub Repository
https://github.com/harshitpandya-cg/node-assignment-3

Server runs at:
http://localhost:5000/

📊 Data Structure :-

Each state follows this structure:
{
  "id": 1,
  "name": "Gujarat",
  "population": 63872399,
  "literacyRate": 78.03,
  "annualBudget": 243965,
  "gdp": 21000000
}

📌 API Routes (13 Total)

🔵 GET

GET /states → Get all states
GET /states/:id → Get state by ID
GET /states/highest-gdp → Get state with highest GDP

🟢 POST

POST /states → Add new state (Status 201)

🟡 PUT

PUT /states/:id → Replace entire state
PUT /states/:id/budget → Update budget
PUT /states/:id/population → Update population

🟣 PATCH

PATCH /states/:id/literacy → Update literacy rate
PATCH /states/:id/gdp → Update GDP
PATCH /states/:id → Partial update fields

🔴 DELETE

DELETE /states/:id → Delete by ID (204)
DELETE /states/name/:stateName → Delete by name (case-insensitive)
DELETE /states/low-literacy/:percentage → Delete states below literacy rate

🧪 Postman Documentation

Public Postman Collection Link:
https://documenter.getpostman.com/view/50839299/2sBXcHhyWY

Includes:
All 13 routes
Sample requests
Sample responses
Automated test scripts

🚀 Deployment Configuration (Render)

Build Command:-
npm install

Start Command:-
node server.js

Server uses:
const PORT = process.env.PORT || 5000;
✅ Status Codes Used

200 → Success

201 → Created

204 → No Content (Deleted)

404 → Not Found

👨‍💻 Author

Harshit Pandya
Assignment 3 – State Statistics Management API
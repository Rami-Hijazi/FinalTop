# 🧠 EventHub Backend (Express + PostgreSQL)

This is the backend for the **EventHub** full-stack event management app. It provides RESTful APIs for managing events, RSVPs, and organizer operations.

---

## 🏗️ Tech Stack

- Node.js + Express
- PostgreSQL (via `pg`)
- `dotenv` for environment variables
- `cors` for cross-origin access
- `morgan` for request logging

---

## 🚀 Getting Started

### 1. Install dependencies

```bash
cd eventhub-server
npm install
2. Create a PostgreSQL database
You can name it eventhubdb or any name you prefer.

3. Configure .env file
Make sure your .env file has the following keys:

ini
Copy
Edit
DB_USER=your_postgres_user
DB_PASSWORD=your_postgres_password
DB_HOST=localhost
DB_PORT=5432
DB_NAME=eventhubdb
PORT=5000
4. Run the server
bash
Copy
Edit
node server.js
🗂️ Project Structure
pgsql
Copy
Edit
eventhub-server/
├── routes/
│   └── events.js         # Event & RSVP related routes
├── db.js                 # PostgreSQL connection
├── server.js             # Main Express server
├── .env                  # Database credentials
├── package.json
└── README.md
📡 API Endpoints
🔗 Base URL: /api/events
Method	Endpoint	Description
GET	/	Get all events
GET	/:id	Get a specific event by ID
POST	/	Create a new event
PUT	/:id	Update an event
DELETE	/:id	Delete an event
POST	/rsvp/:id	RSVP to an event
DELETE	/rsvp/:id/:username	Cancel RSVP
GET	/rsvps/:username	Get events a user RSVP’d to
GET	/organizer/:username	Get events created by organizer

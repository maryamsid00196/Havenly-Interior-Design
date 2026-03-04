# Havenly — Interior Design

A web project for **Havenly**, an interior design destination. It includes a frontend site (home, shop, about) and a Node.js backend with a contact form and MongoDB.

## Project structure

```
InteriorDesigning/
├── index.html          # Shop page (Heavenly)
├── home.html           # Home / landing page
├── About Us.html       # About page
├── style.css           # Styles for shop
├── style1.css          # Styles for home & about
├── backend/
│   ├── index.js        # Express server entry
│   ├── src/
│   │   ├── app.js      # Express app & routes
│   │   └── db/
│   │       └── conn.js # MongoDB connection
│   └── public/         # Static files & contact form
│       ├── index.html
│       ├── script.js
│       └── contactsuccess.html
└── README.md
```

## Tech stack

- **Frontend:** HTML, CSS, Bootstrap 5, Font Awesome, jQuery
- **Backend:** Node.js, Express
- **Database:** MongoDB (Mongoose)

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or newer)
- [MongoDB](https://www.mongodb.com/) running locally (default: `mongodb://localhost:27017`)

## Setup & run

### 1. Backend

```bash
cd backend
npm install
```

Start MongoDB (if not already running), then:

```bash
node index.js
```

Or with auto-reload:

```bash
npx nodemon index.js
```

Server runs at **http://localhost:3000** (or the port in `process.env.PORT`).

### 2. Frontend

Open the HTML files in a browser, or use a simple static server. From the project root:

- **Home:** `home.html`
- **Shop:** `index.html`
- **About:** `About Us.html`
- **Contact:** http://localhost:3000/ (when the backend is running)

## Features

- **Home:** Hero section, services, and “love the space you’re in” messaging
- **Shop:** Categories (Sofas & Sectionals, Accent Seating, Dining Furniture, etc.)
- **About:** Company information
- **Contact:** Form submitted to the backend (stored in MongoDB when implemented)

## Database

The app connects to MongoDB with database name `hevanly` (see `backend/src/db/conn.js`). Ensure MongoDB is running before starting the server.

## License

ISC

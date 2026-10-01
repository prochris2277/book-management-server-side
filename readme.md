# Book Management App API

Backend server for the Book Management App. This API handles users, books, and reading lists using Node.js, Express, MongoDB, and Mongoose.

## Tech Stack

* Node.js
* Express.js
* MongoDB
* Mongoose
* dotenv

## Project Structure

```text
server/
├── src/
│   ├── config/
│   │   └── database.js
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   └── server.js
├── .env
├── .env.example
├── .gitignore
├── package.json
└── README.md
```

## Features

* User management
* Book management
* Reading list management
* MongoDB database integration
* Reading status tracking
* Prevents users from adding the same book to their reading list more than once

## Getting Started

### 1. Clone the repository

```bash
git clone <repository-url>
```

### 2. Navigate to the server

```bash
cd server
```

### 3. Install dependencies

```bash
npm install
```

### 4. Create your environment file

Create a `.env` file in the server folder.

Use `.env.example` as a guide.

Example:

```env
PORT=3000
MONGODB_URI=your_mongodb_connection_string
```

Do not commit your `.env` file to GitHub.

### 5. Start the development server

```bash
npm run start:dev
```

The server should start on:

```text
http://localhost:3000
```

## Environment Variables

| Variable      | Description               |
| ------------- | ------------------------- |
| `PORT`        | Port the server runs on   |
| `MONGODB_URI` | MongoDB connection string |

## Database

The application uses MongoDB as its database and Mongoose to define schemas, models, relationships, and validation rules.

The main models include:

* `User`
* `Book`
* `ReadingList`

The `ReadingList` model connects users with books and stores their reading status.

## Development

During development, use:

```bash
npm run dev
```

Make sure MongoDB is connected successfully before testing API endpoints.

## Security

Environment variables containing sensitive information such as database credentials should be stored in `.env` and excluded from version control.

The `.env.example` file should contain only the required variable names and example values.

## Status

🚧 This project is currently under development.

# Setup-project-NodeJS

This repository provides a standard Node.js backend template with MongoDB Atlas integration.  
It is designed for quick setup and easy extension for small to medium web applications.

## Features

- Express.js server
- MongoDB Atlas connection via Mongoose
- Basic folder structure for scalable backend development
- Sample middleware and error handling
- Ready-to-use sample environment configuration

## Folder Structure (`src`)

- **controllers/**  
  Contains logic for handling API requests and responses (e.g., user management).

- **models/**  
  Defines Mongoose schemas and models for MongoDB collections.

- **routes/**  
  Declares API endpoints and maps them to controller functions.

- **middlewares/**  
  Includes custom middleware for error handling, authentication, logging, etc.

- **config/**  
  Configuration files for environment variables and database connection.

- **app.js / index.js**  
  Entry point for starting the Express server.

## Getting Started

### 1. Clone the repository

```sh
git clone https://github.com/your-username/Setup-project-NodeJS.git
cd Setup-project-NodeJS
```

### 2. Install dependencies

```sh
npm install
```

### 3. Configure environment variables

- Copy `sample.env` to `.env` and fill in your MongoDB Atlas credentials:

```sh
cp sample.env .env
```
- Edit `.env`:
  - `PORT`: Server port (default: 3000)
  - `MONGODB_URL`: Your MongoDB Atlas connection string

### 4. Run the server

```sh
npm start
```
or for development with auto-reload:
```sh
npm run dev
```

## API Sample

The project includes sample user APIs:
- `POST /user` – Create a new user
- `GET /user` – Get all users
- `GET /user/:id` – Get user by ID
- `PUT /user/:id` – Update user by ID

## License

MIT

---

Feel free to fork and extend this template for your own backend projects!

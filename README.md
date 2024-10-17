

# Fullstack Geo-Data App

The Geospatial Data Management Application is a full-stack web application that allows users to manage and visualize geospatial data. Built with a Go backend and a React.js frontend, this application provides functionalities for user authentication, file uploads, map rendering, and shape management using React Leaflet.

 ## Project Live: [Click Here](bit.ly/4dSr9ho)

### Key Features
- User authentication and account management.
- Upload and manage GeoJSON and KML files.
- Render uploaded files on a map using React Leaflet.
- Draw custom shapes on the map and save them to user accounts.
- Edit existing shapes, modifying their geometry and attributes.

### Prerequisites

- Go (version 1.15 or later)
- Node.js (version 14 or later)
- PostgreSQL or SQLite (depending on your choice)
- Git & GitHub

## Installation Instructions

To run the application locally, follow these steps:

### Backend Setup

1. **Clone the Repository:**
   ```bash
   git clone <YOUR_GITHUB_REPOSITORY_LINK>
   cd backend
   ```

2. **Install Dependencies:**
   ```bash
   go mod tidy
   ```

3. **Setup the Database:**
   - Create a PostgreSQL or SQLite database.
   - Configure the database connection in the `.env` file.

4. **Run the Backend:**
   ```bash
   go run main.go
   ```

### Frontend Setup

1. **Navigate to the Frontend Directory:**
   ```bash
   cd ../src
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Run the Frontend:**
   ```bash
   npm run dev
   ```

4. Navigate to `http://localhost:3000` in your browser.

## Usage

1. Navigate to `http://localhost:3000` in your browser.
2. Create a new account or log in to your existing account.
3. Upload GeoJSON or KML files to visualize them on the map.
4. Use the drawing tools to create custom shapes and save them.
5. Edit existing shapes by selecting them on the map.

## API Documentation

### Authentication

- **POST** `/api/register`: Register a new user.
- **POST** `/api/login`: Log in an existing user.
  
### Geospatial Data Management

- **POST** `/api/upload`: Upload GeoJSON or KML files.
- **GET** `/api/data`: Retrieve uploaded geospatial data.
- **PUT** `/api/data/:id`: Update geospatial data.
- **DELETE** `/api/data/:id`: Delete geospatial data.


## Technologies Used

- **Frontend:** React.js, React Leaflet
- **Backend:** Go
- **Database:** PostgreSQL / SQLite

## Deployment

To deploy the application, you can use platforms like Heroku, DigitalOcean, or AWS. Ensure you follow the environment variable configuration and database setup on your chosen platform.

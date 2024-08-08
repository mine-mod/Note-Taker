# Note-Taker App

## Description

The Note-Taker app is a simple application designed to help you keep track of your notes. It allows users to create, view, and delete notes. The app is built with Node.js, Express.js, and utilizes the `uuid` module for unique note identification.

## Features

- **Add Notes**: Create new notes with a title and content.
- **View Notes**: Display a list of all saved notes.
- **Delete Notes**: Remove notes by ID.

## Installation

1. **Clone the Repository**

   ```sh
   git clone https://github.com/mine-mod/Note-Taker.git
   ```

2. **Navigate to the Project Directory**

   ```sh
   cd note-taker
   ```

3. **Install Dependencies**

   Make sure you have [Node.js](https://nodejs.org/) installed. Run the following command to install the required packages:

   ```sh
   npm install
   ```

## Usage

1. **Start the Server**

   Run the following command to start the server:

   ```sh
   npm run start
   ```

   By default, the server will run on port `3001`. You can access the app at `http://localhost:3001`.

2. **Using the Application**

   - Navigate to `http://localhost:3001/notes` to view and add notes.
   - The main page is available at `http://localhost:3001/` for other interactions.

## API Endpoints

- **GET /api/notes**  
  Retrieve all notes.

- **POST /api/notes**  
  Add a new note. The request body should contain the note's title and content.

- **DELETE /api/notes/:id**  
  Delete a note by its ID.

## Project Structure

- `server.js`: The main server file where the Express server is set up.
- `public/`: Directory for static files (HTML, CSS, JavaScript).
  - `notes.html`: HTML file for viewing and adding notes.
  - `index.html`: Main HTML file for the landing page.
- `db/`: Directory for database files.
  - `db.json`: JSON file used to store notes.

## Troubleshooting

- **Module Not Found**: Ensure all dependencies are installed by running `npm install`.
- **File Paths**: Verify that all paths to HTML and JSON files are correct and that files exist in the specified locations.
- **Server Errors**: Check the terminal for error messages. Common issues include file permission problems and incorrect JSON formatting.

## Contributing

If you'd like to contribute to this project, please fork the repository and create a pull request with your changes. Make sure to follow the code style used in the project and include tests for new features.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

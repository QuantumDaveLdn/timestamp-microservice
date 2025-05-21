# Timestamp Microservice

A simple API microservice that parses date strings and returns both Unix timestamp and UTC string formats.

## Features

This microservice provides a date conversion endpoint:

- `GET /api/:date?` - Accepts a date string and returns both Unix and UTC formats
  - If no date is provided, returns the current date
  - Accepts both Unix timestamps and valid date strings
  - Returns error if the date string is invalid

## Example Usage

- `/api/2015-12-25`
- `/api/1451001600000`
- `/api/` (returns current date)

## Example Output

```json
{
  "unix": 1451001600000,
  "utc": "Fri, 25 Dec 2015 00:00:00 GMT"
}
```

## Technologies Used

- Node.js
- Express.js

## Setup and Installation

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Start the server:
   ```
   npm start
   ```
4. Visit `http://localhost:3000` in your browser

## Project Structure

- `index.js` - The main application file with the server configuration and route handling
- `public/style.css` - Styling for the front-end
- `views/index.html` - Front-end interface

## License

This project is part of the freeCodeCamp Backend Development and APIs certification.

*This repository demonstrates my systematic approach to learning database technologies as I build toward my ultimate goal of becoming an AI engineer. Understanding database systems is crucial for developing and deploying robust AI applications.*

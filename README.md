# File Metadata Microservice

## Overview
This is a **File Metadata Microservice** built with **Node.js** and **Express.js**. It allows users to upload a file and returns metadata about the file, including its **name, type, and size**.

## Features
- Users can upload a file using a form.
- Returns a JSON response with file metadata:
  - `name`: Original file name
  - `type`: MIME type of the file
  - `size`: File size in bytes
- Uses **Multer** for handling file uploads.

## Tech Stack
- **Node.js**
- **Express.js**
- **Multer (for file uploads)**

## Installation & Usage

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/file-metadata-microservice.git
cd file-metadata-microservice
```

### 2. Install dependencies
```bash
npm install
```

### 3. Run the server
```bash
node server.js
```
Or use **nodemon** for live reloading:
```bash
npx nodemon server.js
```

### 4. Upload a file
- Open your browser and go to:
  ```
  http://localhost:3000
  ```
- Upload a file through the provided form.
- The server will return a JSON response with file details.

## API Endpoint
### **POST /upload**
#### Request:
- **Form Data** with a file input (name attribute: `upfile`).

#### Response (JSON Example):
```json
{
  "name": "example.png",
  "type": "image/png",
  "size": 34567
}
```

## Deployment
- Deploy using **Render, Replit, Vercel, or Gitpod**.
- Make sure to use `process.env.PORT` for the port configuration.

## License
This project is open-source under the **MIT License**.

---
**Happy coding! 🚀**


# How to Run Your index.html on a Localhost Server

This tutorial will show you how to serve your website locally using a simple HTTP server. This is useful for development and testing.

## Method 1: Using Python

Recommended, No Install Needed on macOS because Python 3 comes pre-installed on most macOS and Linux systems, so you don't need to install anything extra. 

On Windows, you may need to install Python manually from https://www.python.org/ if it is not already installed.

1. **Open Terminal**
    - Navigate to your project folder. For example:
       ```sh
       cd /path/to/your/project/folder
       ```

2. **Start the Server**
   - Run the following command:
     ```sh
     python3 -m http.server 8000
     ```
   - This will start a server at port 8000.

3. **Open in Browser**
   - Go to [http://localhost:8000](http://localhost:8000) in your web browser.
   - You should see your `index.html` file.

---

## Method 2: Using Node.js (Alternative)

1. **Install http-server (if you have Node.js installed)**
   ```sh
   npm install -g http-server
   ```

2. **Start the Server**
   ```sh
   http-server .
   ```
   - By default, this will serve your files at [http://localhost:8080](http://localhost:8080)

---

## Stopping the Server
- To stop the server, go back to your terminal and press `Ctrl + C`.

---

## Why Use a Local Server?
- Some browser features (like module imports, AJAX, etc.) require files to be served over HTTP.
- Avoids browser security restrictions when opening files directly.

---



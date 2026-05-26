# local-webserver-
setup a local webserver
## Local Web Server Setup Report

---

### 1. Executive Summary

This report documents the successful setup and verification of a local HTTP web server on a Windows environment. The server was initialized using Python's built-in networking modules to serve static web assets locally for development purposes.

---

### 2. Environment & Configuration

* **Operating System:** Windows
* **Root Directory:** `D:\website`
* **Server Technology:** Python 3 (`http.server` module)
* **Local Port:** `8000`
* **Default Document:** `index.html`

---

### 3. Implementation Steps

#### Step 1: Server Initialization

The Command Prompt was navigated to the project root directory, and the local server was initialized using the following command:

```cmd
D:\website>python -m http.server 8000

```

> **Server Output:** `Serving HTTP on :: port 8000 (http://[::]:8000/) ...`

#### Step 2: Deployment & Browser Verification

The network loopback address was used to access the local environment via a standard web browser at the following address:

```text
http://localhost:8000/

```

---

### 4. Results & Verification

The server successfully handled the incoming request and resolved the default file structure.

* **Status:** **SUCCESS**
* **Rendered Content:** The browser correctly interpreted the root `index.html` file, rendering the heading text:
> **"Hello World! My Windows web server is working!"**


* **Logs:** The backend terminal accurately captured incoming `GET` requests with a `200 OK` status code, confirming stable data transmission between the local host and the browser client.

---

### 5. Next Steps & Recommendations

With the local hosting environment fully operational, the following development workflow is recommended:

1. **Frontend Modification:** Modify or expand the `index.html` file inside `D:\website` using a text editor (e.g., VS Code or Notepad).
2. **Styling and Logic:** Introduce CSS (`.css`) and JavaScript (`.js`) files into the directory to build out the website's interface and functionality.
3. **Session Management:** Maintain the Command Prompt window in an open state to keep the port active during the development cycle. Turn off the server using `Ctrl + C` when development concludes.

# **Setting Up React Using `create-react-app` in VS Code**
## **Step 1: Install Required Software**
Before you can create a React app, ensure you have the following installed:

### ✅ **1. Install Node.js**
- Go to [https://nodejs.org/](https://nodejs.org/)
- Download **LTS (Long-Term Support) version**.
- Run the installer and follow the instructions.
- After installation, check if Node.js and npm (Node Package Manager) are installed by opening a terminal (Command Prompt or VS Code Terminal) and typing:

  ```sh
  node -v
  npm -v
  ```

  You should see version numbers for both.

### ✅ **2. Install VS Code**
- Download and install **VS Code** from [https://code.visualstudio.com/](https://code.visualstudio.com/).

### ✅ **3. Install Git (Optional but Recommended)**
- Go to [https://git-scm.com/downloads](https://git-scm.com/downloads).
- Download and install Git (default settings are fine).
- Check if Git is installed by running:

  ```sh
  git --version
  ```

---

## **Step 2: Create a New React App**
Once everything is installed, follow these steps:

### **1. Open VS Code**
- Launch **VS Code**.
- Open the **Terminal** in VS Code:
  - Windows: `Ctrl + ~`
  - Mac: `Cmd + ~`
  - Or go to **View > Terminal**.

### **2. Navigate to Your Projects Folder**
- In the terminal, navigate to the folder where you want to create your React app.  
  Example:

  ```sh
  cd Documents
  ```

  If you need to create a new folder:

  ```sh
  mkdir ReactApps
  cd ReactApps
  ```

### **3. Create a New React App**
- Run the following command:

  ```sh
  npx create-react-app my-app
  ```

  - `npx` runs the latest version of `create-react-app` without installing it globally.
  - Replace `my-app` with your project name (no spaces, use dashes or underscores if needed).

- Wait for the installation to complete. This may take a few minutes.

### **4. Open the Project in VS Code**
- Once the installation is done, navigate into the project folder:

  ```sh
  cd my-app
  ```

- Open the project in VS Code:

  ```sh
  code .
  ```

---

## **Step 3: Run the React App**
Now, start the development server:

```sh
npm start
```

- Your browser should open automatically at `http://localhost:3000/` with the React welcome page.

---

## **Step 4: Modify the App**
- Open `src/App.js` in VS Code.
- Replace the default content inside the `<div className="App">` tag.
- Save and check the browser to see updates.

---

## **Step 5: Stop the Server**
- To stop the development server, go back to the terminal and press:
  - **Windows/Linux:** `Ctrl + C`
  - **Mac:** `Cmd + C`

---

## **Troubleshooting**
### ❌ `npx: command not found`
- Ensure you installed Node.js properly.
- Try running:

  ```sh
  npm install -g npx
  ```

### ❌ `create-react-app: command not found`
- Use `npx create-react-app my-app` instead of `create-react-app my-app`.
- Ensure you have the latest Node.js version.

### ❌ `npm start` doesn’t work
- Try running:

  ```sh
  npm install
  ```

- If errors persist, delete `node_modules` and `package-lock.json`:

  ```sh
  rm -rf node_modules package-lock.json
  npm install
  ```

  Then restart the app:

  ```sh
  npm start
  ```

---

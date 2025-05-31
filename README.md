# React + Spring Boot Web Application

This is a full-stack web application built with **React** (frontend) and **Spring Boot** (backend). The frontend communicates with the backend via RESTful APIs.

---

## 🧾 Features

- Modern UI built with React
- RESTful API with Spring Boot
- Gradle-based backend
- Development servers for both frontend and backend

---

## 📁 Project Structure

project-root/
├── backend/ # Spring Boot project (Gradle)
└── frontend/ # React project (Vite or Create React App)



---

## ⚙️ Requirements

Make sure the following tools are installed on your system:

- **Java Development Kit (JDK)** 17 or later  
  [Download JDK](https://adoptium.net/)
- **Gradle** (optional, if not using the wrapper)  
  [Download Gradle](https://gradle.org/install/)
- **Node.js** and **npm**  
  [Download Node.js](https://nodejs.org/) (npm comes bundled)

---

## 🚀 Installation and Running

### 1. Clone the Repository

```bash
git clone https://github.com/hoangphatdev/SoccerStore
cd your-project-name
2. Start the Backend (Spring Boot)
Navigate to the backend directory and run:

cd backend
./gradlew bootRun       # For Linux/macOS
gradlew.bat bootRun     # For Windows
This will start the Spring Boot backend server at:
http://localhost:8080

3. Start the Frontend (React)
Navigate to the frontend directory and run:


cd ../frontend
npm install
npm run dev
This will start the React development server at:
http://localhost:5173 (Vite)
or http://localhost:3000 (Create React App)

🔄 Connecting Frontend with Backend
To enable the React app to send requests to the Spring Boot server during development, configure a proxy.

If using Vite:
In vite.config.js:


export default {
  server: {
    proxy: {
      '/api': 'http://localhost:8080'
    }
  }
}
If using Create React App:
In package.json:


"proxy": "http://localhost:8080"
📌 Notes
Make sure both frontend and backend are running simultaneously.

Use your browser's developer tools or console to check for connection or CORS issues.

If needed, configure CORS in your Spring Boot application.

📝 License
This project is for educational purposes only.
Feel free to modify and extend it as needed.

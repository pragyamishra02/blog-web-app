# MERN Blog App

This is a **full-stack blog application** built using the **MERN stack** (MongoDB, Express.js, React.js, and Node.js). It allows users to create and display blog posts with a modern, fully responsive user interface.  

---

## 🚀 Features
✅ Create, Read, and Display Blogs  
✅ Fully Responsive Design  
✅ Modern UI with React and Tailwind CSS  
✅ RESTful API with Express.js and MongoDB  
✅ State Management with React Hooks  
✅ Modular Codebase  

---

## 🏗️ Project Structure
```
├── blog-app
│   ├── backend
│   │   ├── config
│   │   │   └── db.js
│   │   ├── controllers
│   │   │   └── blogController.js
│   │   ├── models
│   │   │   └── blogModel.js
│   │   ├── routes
│   │   │   └── blogRoutes.js
│   │   ├── .env
│   │   ├── server.js
│   │   ├── package.json
│   ├── frontend
│   │   ├── public
│   │   ├── src
│   │   │   ├── components
│   │   │   │   ├── Blog.js
│   │   │   │   ├── CreateBlog.js
│   │   │   │   └── BlogList.js
│   │   │   ├── context
│   │   │   │   └── BlogContext.js
│   │   │   ├── pages
│   │   │   │   ├── Home.js
│   │   │   │   ├── BlogPage.js
│   │   │   ├── services
│   │   │   │   └── blogService.js
│   │   │   ├── App.js
│   │   │   ├── index.js
│   │   │   └── styles.css
│   │   ├── .env
│   │   ├── package.json
│   └── README.md
```

---

## 🛠️ Technologies Used
### **Frontend:**
- React.js  
- Axios  
- React Router  
- Tailwind CSS  

### **Backend:**
- Node.js  
- Express.js  
- MongoDB  
- Mongoose  
- dotenv  

---

## 📝 Installation and Setup
### **1. Clone the repository:**
```bash
git clone https://github.com/your-username/blog-app.git
```

### **2. Backend Setup:**
Navigate to the backend folder:
```bash
cd blog-app/backend
```
Install dependencies:
```bash
npm install
```
Create a `.env` file:
```plaintext
MONGO_URI = mongodb://localhost:27017/blog-app
PORT = 5000
```
Start the backend:
```bash
npm start
```

---

### **3. Frontend Setup:**
Navigate to the frontend folder:
```bash
cd ../frontend
```
Install dependencies:
```bash
npm install
```
Create a `.env` file:
```plaintext
REACT_APP_API_URL = http://localhost:5000/api
```
Start the frontend:
```bash
npm start
```

---

## ✅ API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET`  | `/api/blogs` | Get all blogs |
| `POST` | `/api/blogs` | Create a new blog |
| `GET`  | `/api/blogs/:id` | Get a single blog by ID |

---

## 📂 Folder Structure Explanation
### **Backend**  
- `config/db.js` – MongoDB connection setup  
- `controllers/blogController.js` – API logic for handling blogs  
- `models/blogModel.js` – Mongoose schema for blogs  
- `routes/blogRoutes.js` – API routes  
- `server.js` – Main Express.js setup  

### **Frontend**  
- `components/Blog.js` – Blog component  
- `components/CreateBlog.js` – Form to create a new blog  
- `services/blogService.js` – Axios API service  
- `App.js` – Main router setup  
- `pages/Home.js` – Home page with blog list  

---

## 🌟 Future Enhancements
- ✅ Add authentication (signup/login)  
- ✅ Add comments and likes on blogs  
- ✅ Improve error handling and form validation  

---

## 🔥 Key Code Snippets
### **Backend Example: Create Blog Endpoint**
```javascript
// routes/blogRoutes.js
const express = require('express');
const router = express.Router();
const { createBlog } = require('../controllers/blogController');

router.post('/', createBlog);

module.exports = router;
```

### **Frontend Example: Axios API Call**
```javascript
// services/blogService.js
import axios from 'axios';

const API_URL = 'http://localhost:5000/api/blogs';

export const getBlogs = async () => {
  const response = await axios.get(API_URL);
  return response.data;
};
```

---

## 🎯 Best Practices Followed
✅ Clean and modular code structure  
✅ Proper state management using React Hooks  
✅ Responsive design using Tailwind CSS  
✅ API error handling and validation  
✅ Secure environment variables  

---

## 👨‍💻 How to Contribute
1. Fork the repository  
2. Create a new branch (`git checkout -b feature-branch`)  
3. Commit your changes (`git commit -m 'Added feature'`)  
4. Push to the branch (`git push origin feature-branch`)  
5. Create a Pull Request  

---

## ⚠️ Troubleshooting
| Issue | Solution |
|-------|----------|
| MongoDB connection error | Ensure MongoDB is running locally |
| CORS error | Add CORS headers in `server.js` |
| Frontend not loading | Ensure the backend is running properly |

---

## 📜 License
This project is licensed under the **MIT License**.

---

## 📧 Contact
If you have any questions or suggestions, feel free to reach out:  
📩 **pragya.mishra01212@gmail.com**  
🌐 **[GitHub](https://github.com/pragyamishra02)**  


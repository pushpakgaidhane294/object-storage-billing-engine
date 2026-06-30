# 📦 Object Storage Billing Engine

A cloud storage billing simulation system built using **C++**, **Crow Framework**, **HTML**, **CSS**, and **JavaScript**. The project allows users to register, log in, upload file information, monitor storage usage, and generate storage bills through REST APIs.

---

## 🚀 Features

- 👤 User Registration
- 🔐 User Login Authentication
- 📂 File Upload Simulation
- 📊 Storage Usage Monitoring
- 💰 Automatic Bill Calculation
- 📜 Usage Log Management
- 🌐 REST API Integration
- 💾 Data Storage using Text Files

---

## 🛠️ Tech Stack

### Frontend
- HTML5
- CSS3
- JavaScript

### Backend
- C++
- Crow Framework
- REST APIs

### Build Tools
- CMake
- Ninja
- MinGW (GCC)

### Data Storage
- users.txt
- objects.txt
- logs.txt

---

## 📁 Project Structure

```
object-storage-billing-engine/
│
├── src/
│   └── main.cpp
│
├── include/
│   └── crow/
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── build/
│
├── users.txt
├── objects.txt
├── logs.txt
│
├── CMakeLists.txt
└── README.md
```

---

## ⚙️ Installation

### 1. Clone Repository

```bash
git clone https://github.com/pushpakgaidhane294/object-storage-billing-engine.git
```

---

### 2. Go to Project Folder

```bash
cd object-storage-billing-engine
```

---

### 3. Create Build Folder

```bash
mkdir build
cd build
```

---

### 4. Generate Build Files

```bash
cmake ..
```

---

### 5. Build Project

```bash
cmake --build .
```

---

### 6. Run Server

```bash
server.exe
```

Server starts at

```
http://localhost:18080
```

---

## 🌐 REST APIs

### Register User

```
POST /register
```

Example JSON

```json
{
    "name":"Pushpak",
    "email":"pushpak@gmail.com",
    "password":"123456"
}
```

---

### Login

```
POST /login
```

Example JSON

```json
{
    "email":"pushpak@gmail.com",
    "password":"123456"
}
```

---

### Upload File

```
POST /upload
```

Example JSON

```json
{
    "email":"pushpak@gmail.com",
    "file_name":"Resume.pdf",
    "file_type":"pdf",
    "file_size":1200
}
```

---

### Check Storage

```
GET /storage/{email}
```

Example

```
/storage/pushpak@gmail.com
```

---

### Generate Bill

```
GET /bill/{email}
```

Example

```
/bill/pushpak@gmail.com
```

---

### View Users

```
GET /users
```

---

## 💰 Billing Formula

```
Bill = (Storage Used in MB × ₹0.05)
       +
       Number of Uploads
```

Example

Storage = **25 MB**

Uploads = **8**

```
Bill = (25 × 0.05) + 8
     = ₹9.25
```

---

## 📂 Data Files

The application stores data locally using text files.

| File | Purpose |
|------|----------|
| users.txt | User Information |
| objects.txt | Uploaded File Details |
| logs.txt | Activity Logs |

---

## 🧪 Testing

The backend APIs were tested using:

- Postman
- Browser Fetch API
- JavaScript Fetch Requests

---

## 📸 Screenshots

Add screenshots here:

- Home Page
- Registration
- Login
- Upload
- Storage Usage
- Bill Generation
- Backend Terminal

---

## 🔮 Future Improvements

- 📤 Real File Upload
- 🗑 Delete Uploaded Files
- 📄 PDF Invoice Generation
- 📊 Dashboard Analytics
- 🗄 MySQL Database Integration
- ☁ AWS S3 Integration
- 🔑 JWT Authentication
- 👥 User Roles (Admin/User)

---

## 🎯 Learning Outcomes

Through this project, I learned:

- REST API Development in C++
- Crow Framework
- Frontend-Backend Integration
- CMake Build System
- JSON Parsing
- File Handling in C++
- Cloud Storage Billing Logic
- API Testing using Postman

---

## 👨‍💻 Author

**Pushpak Gaidhane**

# 📌 Complaint Management System – Java (Mini Project)

This is a Java-based Complaint Management System that allows users to register, log in, submit complaints, and view the status of their complaints.  
Admins can view all submitted complaints and update their status.  
The project uses **Java OOP**, **File Handling**, **Custom Exceptions**, and **Java Swing GUI**.

---

## 🚀 Features

### 👤 User Module
- Register a new account  
- Login using username & password  
- Submit a complaint  
- View complaint status  

### 🛠️ Admin Module
- Login using fixed admin credentials  
  - **Username:** admin  
  - **Password:** admin123  
- View all complaints  
- Update complaint status  

### 💾 Storage
The system uses **text files** for storage:
- `users.txt` → Stores registered users  
- `complaints.txt` → Stores submitted complaints and their status  

---

## 🗂️ Project Structure

```
Complaint-Management-System-Java/
│
├── src/
│   ├── AdminPanel.java
│   ├── AdminService.java
│   ├── Complaint.java
│   ├── ComplaintService.java
│   ├── DuplicateUserException.java
│   ├── FileAccessException.java
│   ├── FileManager.java
│   ├── TextFileManager.java
│   ├── GuiMain.java
│   ├── Main.java
│   ├── MainFrame.java
│   ├── User.java
│   ├── UserPanel.java
│   ├── UserService.java
│   ├── UserNotFoundException.java
│
├── data/
│   ├── users.txt
│   ├── complaints.txt
│
├── Output.docx
├── Project-Presentation.pptx
└── README.md
```

---

## 🧩 Class Overview

### 🔹 Model Classes
- **User.java** → Stores username & password  
- **Complaint.java** → Stores complaint ID, user, category, description & status  

### 🔹 Service Classes
- **UserService.java** → Handles registration & login  
- **AdminService.java** → Handles admin login using fixed credentials  
- **ComplaintService.java** → Adds, reads & updates complaints  

### 🔹 File Handling
- **FileManager.java** → Base class for file reading/writing  
- **TextFileManager.java** → Actual implementation using text files  

### 🔹 Custom Exceptions
- DuplicateUserException  
- UserNotFoundException  
- FileAccessException  

### 🔹 GUI Classes (Java Swing)
- **MainFrame.java** → Main window  
- **UserPanel.java** → User dashboard  
- **AdminPanel.java** → Admin dashboard  
- **GuiMain.java** → GUI entry point  

### 🔹 Console Version  
- **Main.java** → Text-based menu-driven version  

---

## ▶️ How to Run the Project

### **Run GUI Version**
Run:
GuiMain.java

### **Run Console Version**
Run:
Main.java

---

## 📂 Data File Format

### users.txt
username,password

### complaints.txt
id|username|category|description|status

---

## 📘 Future Enhancements
- Replace text files with MySQL database  
- Add password hashing  
- Add email/SMS notifications  
- Add filtering/sorting of complaints in admin panel  


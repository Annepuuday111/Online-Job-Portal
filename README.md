# 🌐 Online Job Portal

<p align="center">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Backend-Django-green?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/Database-PostgreSQL-blue?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Frontend-HTML5%20%7C%20CSS3-orange?style=for-the-badge&logo=html5" />
</p>

---

## 🚀 Live Demo / Deployment  

<p align="center">
🔗 *[Link to Live Demo if deployed]*  
</p>

---

## 🏗️ About the Project  

The **Online Job Portal** is a modern web application built with **Django**, **PostgreSQL**, **HTML**, and **CSS**.  
It serves as a centralized platform for **students**, **companies**, and **admins** to manage job applications efficiently.  

> 💡 *"Connecting talented students with leading companies seamlessly"*  

**Key Highlights:**  
- 🌟 Admin-controlled system to manage companies and jobs  
- ⚡ Companies can post jobs after admin approval  
- 📱 Students can browse jobs, apply, and track application status  
- 🎯 Real-time notifications for selection/rejection  
- 🛡️ Secure registration and role-based access  

---

## ✨ Features  

| 🧩 Feature | 📋 Description |
|------------|----------------|
| **👨‍💼 Admin Module** | Accept/reject company registrations, manage job postings, and oversee student applications |
| **🏢 Company Module** | Register, post job notifications, view student applicants, shortlist candidates, and send messages |
| **🎓 Student Module** | Register, view approved company profiles, browse jobs, apply, and track application status |
| **📬 Messaging** | Companies can send selection or rejection messages to students |
| **📱 Responsive Design** | Mobile-friendly interface across all devices |
| **🔒 Role-Based Access** | Secure login for Admin, Company, and Student roles |

---

## 🧱 Tech Stack  

| Technology | Description |
|------------|-------------|
| 🐍 **Python & Django** | Backend framework handling server-side logic, routing, and database interactions |
| 🐘 **PostgreSQL** | Relational database storing user profiles, jobs, applications, and messages |
| 🎨 **HTML5 & CSS3** | Frontend layout, responsive design, and styling |
| ⚙️ **JavaScript (Optional)** | Dynamic interactions and UI enhancements |
| 🌐 **Bootstrap (Optional)** | CSS framework for responsive and modern components |

---

## 🖼️ Module Screenshots  

### 1️⃣ Admin Dashboard  
- View and approve company registrations  
- Monitor job postings  
- Manage student applications  

### 2️⃣ Company Dashboard  
- Post new job notifications  
- View student applicants  
- Shortlist candidates and send messages  

### 3️⃣ Student Dashboard  
- Browse available jobs and companies  
- Apply to jobs and track application status  
- Receive notifications from companies  

---

## 🔧 How to Run Locally  

```bash
# Clone the repository
git clone https://github.com/YourUsername/CollegeJobPortal.git

# Navigate to project directory
cd CollegeJobPortal

# Create a virtual environment
python -m venv venv

# Activate the environment
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Apply migrations
python manage.py migrate

# Run the development server
python manage.py runserver

# Open the browser at http://127.0.0.1:8000

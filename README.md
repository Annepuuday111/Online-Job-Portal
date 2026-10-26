<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF6B6B,35:FFA94D,70:4DABF7,100:845EF7&height=200&section=header&text=Online%20Job%20Portal&fontSize=44&fontColor=ffffff&fontAlignY=36&animation=fadeIn&desc=Connecting%20students%20with%20companies%20%E2%80%94%20Django%20%2B%20PostgreSQL&descSize=16&descAlignY=58" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=845EF7&center=true&vCenter=true&width=700&lines=Students+browse+and+apply+for+jobs;Companies+post+jobs+after+approval;Admin+approves+or+rejects+companies" alt="Typing SVG"/>

<br/>

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white"/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white"/>
<img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white"/>
<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>

<br/>

<img src="https://img.shields.io/badge/Status-Completed-20C997?style=for-the-badge"/>
<img src="https://img.shields.io/github/stars/Annepuuday111/Online-Job-Portal?style=for-the-badge&color=845EF7"/>
<img src="https://img.shields.io/github/last-commit/Annepuuday111/Online-Job-Portal?style=for-the-badge&color=4DABF7"/>
<img src="https://img.shields.io/github/repo-size/Annepuuday111/Online-Job-Portal?style=for-the-badge&color=FF6B6B"/>

<br/><br/>

[About](#-about) • [Features](#-features) • [Tech Stack](#️-tech-stack) • [Project Structure](#-project-structure) • [Getting Started](#-getting-started) • [Author](#-author)

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 📖 About

The **Online Job Portal** is a web application built with **Django**, **PostgreSQL**, **HTML** and **CSS**. It is a single place for **students**, **companies** and **admins** to handle job postings and applications.

> 💡 *"Connecting talented students with leading companies seamlessly"*

Companies register and wait for admin approval before they can sign in and post jobs. Students sign up, browse openings, read job details and apply with their resume while the job's application window is open. The admin reviews companies and manages applicants.

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## ✨ Features

| Role | What they can do |
| :--- | :--- |
| 🎓 **Student** | Sign up with photo, log in, edit profile, browse all jobs (newest first), view job details, apply with a resume upload; jobs already applied for are marked; applications are blocked before the start date and after the end date |
| 🏢 **Company** | Register (status starts as *pending*), log in once approved, edit profile, add and edit jobs (title, salary, dates, experience, location, skills, description), upload a logo per job, see applicants and open their resumes |
| 🛡️ **Admin** | Log in with a Django superuser account, view pending / accepted / rejected / all companies, accept or reject a company, delete companies, view and delete applicants |
| 📋 **Tables** | Admin lists use jQuery DataTables with copy, Excel, CSV and PDF export buttons |

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🛠️ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=python,django,postgres,bootstrap,jquery,html,css&theme=light"/>

</div>

| Layer | Technology |
| :--- | :--- |
| Backend | Python, Django 5.0 (`django.contrib.auth` for login) |
| Database | PostgreSQL (`psycopg2`) |
| Frontend | Django templates, HTML5, CSS3, Bootstrap 5, Font Awesome |
| Tables | jQuery DataTables + Buttons (JSZip, pdfmake) |
| Media | Pillow (`ImageField` uploads to `media/`) |

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 📂 Project Structure

```text
Online-Job-Portal/
└── onlinejobportal/
    ├── onlinejobportal/   # settings.py, urls.py, wsgi.py, asgi.py
    ├── jobs/              # Applicant, Company, Job, Application models; views; urls
    ├── templates/         # student, company and admin pages + navbars
    ├── static/
    │   └── css/style.css
    ├── media/             # uploaded photos, logos and resumes
    └── manage.py
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- PostgreSQL running locally

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Annepuuday111/Online-Job-Portal.git
   cd Online-Job-Portal/onlinejobportal
   ```
2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate      # Windows: venv\Scripts\activate
   ```
3. **Install dependencies**
   ```bash
   pip install "Django>=5.0,<5.1" psycopg2-binary Pillow
   ```
4. **Create the database** and update `DATABASES` in `onlinejobportal/settings.py` with your own credentials
   ```sql
   CREATE DATABASE jobportal;
   ```
5. **Apply migrations and create the admin account**
   ```bash
   python manage.py migrate
   python manage.py createsuperuser
   ```
6. **Run the server**
   ```bash
   python manage.py runserver
   ```
   Open http://127.0.0.1:8000. Admin login is at `/admin_login/`, company login at `/company_login/`, student login at `/user_login/`.

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🗺️ Roadmap

- [ ] Show application status (selected / rejected) to students
- [ ] Move database credentials to environment variables
- [ ] Add a `requirements.txt`

## 🤝 Contributing

Contributions are welcome. Fork the repo, create a branch (`git checkout -b feature/my-change`), commit your work and open a pull request.

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 👨‍💻 Author

<div align="center">

### Annepu Uday Kumar

<a href="https://github.com/Annepuuday111"><img src="https://img.shields.io/badge/GitHub-Annepuuday111-845EF7?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://annepuudaykumar.netlify.app"><img src="https://img.shields.io/badge/Portfolio-annepuudaykumar-FF6B6B?style=for-the-badge&logo=netlify&logoColor=white"/></a>

</div>

<br/>

<div align="center">⭐ If you like this project, give it a star!</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:845EF7,35:4DABF7,70:FFA94D,100:FF6B6B&height=120&section=footer" width="100%"/>

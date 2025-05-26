# TheatreCMS3 🎭  
## ASP.NET MVC Theatre Management App

> Built as part of a real-world apprenticeship through **Prosper IT Consulting** via *The Tech Academy*, TheatreCMS3 is a dynamic ASP.NET MVC web application created to manage blog content for a fictional theatre group: **Theatre Vertigo**. This project follows Agile/Scrum methodology with full CRUD support, SQL integration, responsive UI, and modern dev tools.

---

## 📑 Table of Contents

* [Project Overview](#project-overview)
* [Key Features](#key-features)
* [User Interface](#user-interface)
* [BlogAuthor and BlogPost Models](#blogauthor-and-blogpost-models)
* [Blog Authors Card](#blog-authors-card)
* [BlogAuthor Views](#blogauthor-views)
* [BlogAuthor Delete Example](#blogauthor-delete-example)
* [Controllers and Forms](#controllers-and-forms)
* [BlogAuthor Controller Logic](#blogauthor-controller-logic)
* [Git and Version Control](#git-and-version-control)
* [Azure DevOps and Agile Process](#azure-devops-and-agile-process)
* [SQL Server and Database Integration](#sql-server-and-database-integration)
* [Final Thoughts](#final-thoughts)

---

## Project Overview 🚀

**TheatreCMS3** is a comprehensive theatre content management system built using **C#, ASP.NET MVC**, and **Entity Framework**.  
My role in this project was to manage the platform for *Blog Authors* that enables staff to manage said authors and their associated posts through a tab-based UI that displays Author Detail Cards and Blog Posts.  
I also worked on the UI/UX to create an enjoyable user interface and experience through clean navigation and user functionality.  
I'm proud of the work the team and I accomplished over the 2-week Sprint, providing deliverables on schedule and to client satisfaction.

---

## Key Features 💡

- ✅ Full CRUD for Blog Authors and Blog Posts  
- 📆 DateTime picker support for `Joined` and `Left` values  
- 🎨 Tabbed interface for toggling between Author Info & Posts  
- 📱 Responsive design with custom Bootstrap 4 styling  
- 🖼️ Avatar images for author branding  
- 🔗 Social media icons (Font Awesome)  
- 💥 Confirm deletion with visual warning  
- 🧠 Model validation & error feedback  

---

## User Interface 🖥️

### Home Page  
![Home Page Spotlight](assets/screenshots/Home.png)

---

## BlogAuthor and BlogPost Models 🧠

Example Models:  
![BlogAuthors Models](assets/screenshots/Models.png)

---

## Blog Authors Card 🧑‍🎨

![Blog Authors List](assets/screenshots/BlogAuthors.png)

---

## BlogAuthor Views 🧾

CRUD Views:  
![BlogAuthors Views](assets/screenshots/CreateEditViews.png)

---

## BlogAuthor Delete Example 🗑️

### Details/Delete Confirmation  
![BlogAuthor Delete Confirmation](assets/screenshots/Haruki_Murakami_Delete.png)  
![BlogAuthors Views](assets/screenshots/DeleteDetailsViews.png)

---

## Controllers and Forms 🧠

### Create Blog Author Form (UI)  
![Create BlogAuthor Form](assets/screenshots/Create2.png)

### Create Blog Author Form (Code)  
![Create BlogAuthor Form](assets/screenshots/Create.png)

---

## BlogAuthor Controller Logic 🧠

![BlogAuthors Controller](assets/screenshots/Controllers.png)

---

## Git and Version Control 🔀

Version control handled using **Git** and hosted on **GitHub**:

- Feature branching  
- Pull Requests (PRs) for reviews  
- Merge and migration conflict resolution  
- `.gitignore` to exclude secrets and build files  

---

## Azure DevOps and Agile Process 🚀

Managed under a real Agile Scrum framework:

- Sprint Planning & Task Estimation  
- Daily Standups  
- Sprint Retrospectives  
- Azure Boards for tracking progress  

---

## SQL Server and Database Integration 🗃️

Entity Framework with SQL Server used for backend:

- Code-First Migrations  
- SQL Server Explorer to inspect DB schema  
- Example migration command:
  ```bash
  Add-Migration InitialCreate
  Update-Database


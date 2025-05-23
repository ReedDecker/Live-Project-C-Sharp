# 🎭 THEATRE CMS3 — ASP.NET MVC Application

## 🌟 Project Overview

**TheatreCMS3** is a full-scale MVC web application developed in **C#** using the **ASP.NET Framework**. Built during an apprenticeship with **Prosper IT Consulting** as part of The Tech Academy’s developer bootcamp, this project simulates a **content management system for a fictional theatre company**.

This project was developed collaboratively using Agile/Scrum methodologies. As part of the team, I contributed through daily stand-ups, sprint planning, code retrospectives, and completing real-world user stories. The application serves as a powerful learning platform to understand enterprise-grade software architecture and modern development workflows.

![Home Page UI](assets/screenshots/Home.png)
> 🎬 *Main Spotlight Page Displaying Upcoming Productions*

---

## 📚 Table of Contents

- [🎨 Bootstrap Customization](#-bootstrap-customization)
- [🧰 Chrome Dev Tools & Debugging](#-chrome-dev-tools--debugging)
- [🧾 CRUD Functionality](#-crud-functionality)
- [💻 HTML / CSS Styling](#-html--css-styling)
- [📜 JavaScript Features](#-javascript-features)
- [🔀 Git & Version Control](#-git--version-control)
- [🚀 Azure DevOps & Agile Process](#-azure-devops--agile-process)
- [🗃️ SQL Server & Database Integration](#️-sql-server--database-integration)
- [📌 Final Thoughts](#-final-thoughts)

---

## 🎨 Bootstrap Customization

The layout was designed using **Bootstrap** with a customized theme:
- Custom color palette defined in `:root` for consistency.
- Card layouts used for BlogAuthors with responsive elements.
- Navigation bar includes dropdowns and branding.

![Blog Authors Layout](assets/screenshots/BlogAuthors.png)
> 🖼️ *Responsive Blog Author Cards With Custom Buttons and Styling*

---

## 🧰 Chrome Dev Tools & Debugging

Used extensively for:
- Real-time style edits.
- DOM inspection.
- Network request debugging for form actions and AJAX calls.
- JavaScript console debugging for dynamic tab toggles.

---

## 🧾 CRUD Functionality

Implemented via Entity Framework using Code-First Migrations. Each model supports full CRUD:

- **BlogAuthor**: Name, Bio, Joined/Left
- **BlogPost**: Title, Description, BlogPhoto, Published, BlogAuthor link

### ✏️ Example: BlogPost Model

```csharp
public class BlogPost {
    [Key]
    public int BlogPostId { get; set; }
    
    [Required]
    public string Title { get; set; }

    [Required]
    public DateTime Published { get; set; }

    public int BlogAuthorId { get; set; }

    [ForeignKey("BlogAuthorId")]
    public virtual BlogAuthor BlogAuthor { get; set; }
}


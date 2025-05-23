# 🎭 THEATRE CMS3 — ASP.NET MVC Application

## 🌟 Project Overview

**TheatreCMS3** is a full-scale MVC web application developed in **C#** using the **ASP.NET Framework**. Built during an apprenticeship with **Prosper IT Consulting** as part of The Tech Academy’s developer bootcamp, this project simulates a **content management system for a fictional theatre company**.

This project was developed collaboratively using Agile/Scrum methodologies. As part of the team, I contributed through daily stand-ups, sprint planning, code retrospectives, and completing real-world user stories. The application serves as a powerful learning platform to understand enterprise-grade software architecture and modern development workflows.

![Home Page UI](assets/screenshots/Home.png)
> 🎬 *Main Spotlight Page Displaying Upcoming Productions*

## 📚 Table of Contents

- [🎨 Bootstrap Customization](#bootstrap-customization)
- [🧰 Chrome Dev Tools & Debugging](#chrome-dev-tools--debugging)
- [🧾 CRUD Functionality](#crud-functionality)
- [💻 HTML / CSS Styling](#html--css-styling)
- [📜 JavaScript Features](#javascript-features)
- [🔀 Git & Version Control](#git--version-control)
- [🚀 Azure DevOps & Agile Process](#azure-devops--agile-process)
- [🗃️ SQL Server & Database Integration](#sql-server--database-integration)
- [🗑️ BlogAuthor Delete Example](#blogauthor-delete-example)
- [🧠 Controllers & Forms](#controllers--forms)
- [📌 Final Thoughts](#final-thoughts)



## 🎨 Bootstrap Customization

The application uses **Bootstrap** to provide a responsive and polished front-end experience:

- Customized color palette defined using CSS variables in `:root`.
- Unified layout and spacing system with consistent padding, margins, and borders.
- Responsive grid for Blog Author cards and Spotlight images.
- Navbar dropdowns styled to align with theatre branding.

![Blog Authors Layout](assets/screenshots/BlogAuthors.png)
> 🖼️ *Responsive Blog Author Cards With Custom Buttons and Styling*

---

## 🧰 Chrome Dev Tools & Debugging

Chrome DevTools were an essential part of the development workflow:

- **Live CSS tweaking** to preview and debug layout changes.
- **Network tab** to inspect CRUD requests and responses.
- **JavaScript console** for tracing event listeners and DOM state.
- **Mobile simulation** to verify responsiveness and media query breakpoints.

---

## 🧾 CRUD Functionality

All primary data models support full Create, Read, Update, and Delete functionality using **Entity Framework Code First**:

- **BlogAuthor**: Contains Name, Bio, Joined/Left dates.
- **BlogPost**: Contains Title, Description, BlogPhoto URL, Published Date, and Author linkage.

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

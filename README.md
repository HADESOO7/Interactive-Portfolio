# 💎 Manu Kumar - Developer Portfolio

A premium, high-performance personal portfolio website featuring a <br>
**macOS-inspired Glassmorphism UI**, **Bento-Grid layouts**, and **interactive dark/light modes**.

<p>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
</p>

### <a href="portfoliobanaya.netlify.app">View Live Demo 🚀</a>

<br />

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#interface-preview">Interface Preview</a></li>
    <li><a href="#key-features">Key Features</a></li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#technologies-used">Technologies Used</a></li>
    <li><a href="#code-highlight">Code Highlight</a></li>
  </ol>
</details>

---

## 👨‍💻 About The Project

This project is a modern digital resume and portfolio designed to showcase my journey as a **CSE Student** and **Full Stack Developer**. Built without external CSS frameworks, it demonstrates mastery over core web technologies.

The design philosophy focuses on **"Digital Reality"**—blending depth, blur, and motion to create a tactile experience. It features a custom-built theme engine that persists user preferences and a highly responsive layout that adapts from ultrawide monitors to mobile screens.

## 📸 Interface Preview

<div align="center"> 
  <img src="screenshot.png" alt="Portfolio Dark Mode" width="800" />
</div>

> *The interface features a Glassmorphism-inspired "Tahoe" aesthetic with expanding social pills and neon-accented controls.*

## ✨ Key Features

| Feature | Description |
| :--- | :--- |
| **Glassmorphism UI** | Heavy use of `backdrop-filter: blur()` and semi-transparent layers to create depth and hierarchy. |
| **Smart Theme Toggle** | Instantly switches between a deep "OLED Black" mode and a "Frosted White" mode, saving preference to LocalStorage. |
| **Bento Grid Layout** | A modular, responsive grid system for the "Technical Arsenal" section that reorganizes based on screen width. |
| **Interactive Contact** | Custom-built social buttons that expand on hover to reveal details, featuring copy-to-clipboard functionality for email/phone. |
| **Responsive Design** | Fluid typography and flexible containers ensure a perfect experience on Mobile, Tablet, and Desktop. |

## 🛠️ Technologies Used

* **Core:** Semantic HTML5
* **Styling:** CSS3 (Custom Properties/Variables, Flexbox, Grid, Keyframe Animations)
* **Logic:** Vanilla JavaScript (ES6+, DOM Manipulation, LocalStorage API)
* **Assets:** FontAwesome 6, Google Fonts (Inter), Shields.io Badges

## 🚀 Getting Started

To run this project locally on your machine, follow these simple steps.

### Prerequisites
* A modern web browser (Chrome, Firefox, Safari, Edge).

### Installation

1.  **Clone the repository**
    ```sh
    git clone [https://github.com/HADESOO7/Portfolio.git](https://github.com/HADESOO7/Portfolio.git)
    ```
2.  **Navigate to the project directory**
    ```sh
    cd Portfolio
    ```
3.  **Open the file**
    Double-click `index.html` to launch the website in your default browser.

## 🧠 Code Highlight

A look at the CSS logic for the expanding "Social Pills" animation:

```css
/* Expanding Social Pill Animation */
.social-pill {
    width: 50px; 
    height: 50px;
    border-radius: 50px;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    overflow: hidden;
}

.social-pill:hover {
    width: auto; 
    padding: 0 25px; 
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}

/* Specific Brand Gradient on Hover */
.social-pill.instagram:hover {
    background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #fd5949 45%, #d6249f 60%, #285AEB 90%);
    border: none;
}

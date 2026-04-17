# 🌐 Mir Yaseen Ali | Personal Portfolio

<p align="center">
  <img src="src/img/Screenshot 2026-04-16 215040.png" width="800" alt="Portfolio Home Page Screenshot">
</p>

This repository contains the source code and configuration for my professional portfolio. The goal of this project was to build a clean, performant showcase for my technical skills while gaining practical experience with modern frontend frameworks and production cloud deployments.

---

## 🚀 Live Demonstration

<p align="center">
  <a href="https://d3mte3hn7uzxb.cloudfront.net/">
    <img src="https://img.shields.io/badge/View%20Live%20Project-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="Live Project Button">
  </a>
  <br>
  <strong>https://d3mte3hn7uzxb.cloudfront.net/</strong>
</p>

---

## 🛠 Project Blueprint

I structured this project using a standard, component-based frontend approach, focusing on a robust architecture that separation of concerns between structure, style, and deployment.

### 📋 Technical Stack

| Area | Tools Used | Why this was chosen |
| :--- | :--- | :--- |
| **Frontend** | React, JS (ES6+), HTML5 | Allows for component reusability and declarative state management. |
| **Styling** | [Tailwind CSS / CSS3 / SCSS] | Used [Utility classes / Flexbox & Grid] for rapid, responsive layout development. |
| **Hosting** | Amazon S3 | Serverless, durable, and highly cost-effective for static asset storage. |
| **CDN** | Amazon CloudFront | Delivers content globally from edge locations, minimizing latency for users. |

---

## ✨ Design Philosophy & Key Features

<p align="center">
  <img src="projects.png" width="600" alt="Projects Showcase Section">
  <img src="mobile.png" width="200" alt="Mobile View Screenshot" style="margin-left: 20px;">
</p>
<p align="center"><i>Visual breakdown of the Projects Gallery and responsive Mobile layout.</i></p>

### Highlighted Features:

* **⚡ High Performance:** Optimized for fast First Contentful Paint (FCP). I focused on image compression, lazy loading, and asset minimization to ensure swift loading.
* **📱 Fully Responsive:** The UI was designed mobile-first, utilizing fluid layouts and media queries. The gallery cards and navigation adjust seamlessly to desktops, tablets, and phones.
* **📂 Interactive Project Gallery:** Dynamically renders project details. I designed the component to fetch repository data [manually/via API], showcasing live links and code descriptions.

---

## 🏗 Infrastructure and Deployment

<p align="center">
  <img src="https://lucid.app/publicSegments/view/04d4a8e2-04e3-4c6e-81fb-325b15a6b09c/image.png" width="650" alt="AWS Infrastructure Diagram">
</p>
<p align="center"><i>Visualization of the content delivery flow.</i></p>

The infrastructure is built to adhere to AWS well-architected principles:

1.  **Security (Private S3):** The S3 bucket is configured with **public access blocked**. Content is accessed *only* through CloudFront.
2.  **Origin Access Identity (OAI):** A specific CloudFront OAI user is granted exclusive IAM permission to read from the bucket, ensuring the "backend" storage is secured from direct public traffic.
3.  **Global Delivery:** CloudFront caches the application assets (`index.html`, `js`, `css`, `images`) across its global edge location network.

---

## 💻 Technical Setup (Local)

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Gogeta0011/Portfolio-Website.git](https://github.com/Gogeta0011/Portfolio-Website.git)

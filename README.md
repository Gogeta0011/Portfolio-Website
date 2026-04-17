# 🌐 Mir Yaseen Ali — Personal Portfolio

<p align="center">
  <img src="src/img/Screenshot 2026-04-16 215040.png" width="800" alt="Portfolio Home Page Screenshot">
</p>

<p align="center">
  <a href="https://d3mte3hn7uzxb.cloudfront.net/">
    <img src="https://img.shields.io/badge/View%20Live%20Project-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="Live Project">
  </a>
  &nbsp;
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React">
  &nbsp;
  <img src="https://img.shields.io/badge/Amazon_S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white" alt="S3">
  &nbsp;
  <img src="https://img.shields.io/badge/CloudFront-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="CloudFront">
</p>

A performant, fully responsive personal portfolio built with React and deployed on AWS. Designed to showcase my technical skills, project work, and cloud infrastructure experience — all delivered globally via CloudFront CDN.

---

## 🚀 Live Demo

**→ [https://d3mte3hn7uzxb.cloudfront.net/](https://d3mte3hn7uzxb.cloudfront.net/)**

---

## 🛠 Tech Stack

| Area | Technology | Purpose |
| :--- | :--- | :--- |
| **Frontend** | React, JavaScript (ES6+), HTML5 | Component-based architecture with declarative state management |
| **Styling** | CSS3, Flexbox & Grid | Responsive, mobile-first layouts with clean, maintainable styles |
| **Hosting** | Amazon S3 | Serverless static asset storage — durable and cost-effective |
| **CDN** | Amazon CloudFront | Global edge delivery to minimize latency for all users |

---

## ✨ Features

- **⚡ Optimized Performance** — Fast First Contentful Paint (FCP) achieved through image compression, lazy loading, and asset minimization.
- **📱 Fully Responsive** — Mobile-first design using fluid layouts and media queries. Navigation and project cards adapt seamlessly across desktops, tablets, and phones.
- **📂 Interactive Project Gallery** — Dynamically rendered project cards showcasing live links, descriptions, and tech used on each project.

---

## 🏗 AWS Infrastructure

<p align="center">
  <img src="https://lucid.app/publicSegments/view/04d4a8e2-04e3-4c6e-81fb-325b15a6b09c/image.png" width="650" alt="AWS Infrastructure Diagram">
</p>
<p align="center"><i>Content delivery flow from S3 origin through CloudFront edge locations.</i></p>

The deployment follows AWS Well-Architected principles across three layers:

1. **Private S3 Bucket** — All public access is blocked at the bucket level. No assets are ever directly exposed.
2. **Origin Access Identity (OAI)** — A dedicated CloudFront OAI is the only principal granted IAM `s3:GetObject` permission, ensuring the storage layer is completely shielded from direct traffic.
3. **CloudFront CDN** — Caches `index.html`, JS bundles, CSS, and image assets across AWS's global edge network for low-latency delivery worldwide.

---

## 💻 Local Setup

```bash
# 1. Clone the repository
git clone https://github.com/Gogeta0011/Portfolio-Website.git
cd Portfolio-Website

# 2. Install dependencies
npm install

# 3. Start the development server
npm start
```

The app will be available at `http://localhost:3000`.

---

## 📁 Project Structure

```
Portfolio-Website/
├── public/
├── src/
│   ├── components/     # Reusable React components
│   ├── img/            # Static image assets
│   ├── App.js
│   └── index.js
├── package.json
└── README.md
```

---

*Built and deployed by Mir Yaseen Ali*

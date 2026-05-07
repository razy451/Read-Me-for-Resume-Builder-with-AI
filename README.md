Yes — your README had Git merge conflict markers (`<<<<<<< HEAD`, `=======`, `>>>>>>>`) in the tester account and license sections. I cleaned it and made it more polished for GitHub. 

Copy this into `README.md`:

````md
# 🚀 Resume Builder with AI

A modern AI-powered resume builder with live preview, built using React, Vite, Strapi, Clerk, MySQL, and Google Gemini API.

![React](https://img.shields.io/badge/React-Frontend-blue)
![Vite](https://img.shields.io/badge/Vite-Build%20Tool-purple)
![Strapi](https://img.shields.io/badge/Strapi-Backend-indigo)
![Clerk](https://img.shields.io/badge/Clerk-Authentication-green)
![Gemini](https://img.shields.io/badge/Gemini-AI-orange)

---

## ✨ Features

- User authentication with Clerk
- Create, edit, duplicate, delete, archive, publish, and restore resumes
- Dynamic resume sections:
  - Personal Details
  - Summary
  - Work Experience
  - Education
  - Skills
  - Custom Sections
- Theme customization:
  - Colors
  - Fonts
  - Spacing
  - Line height
- Live resume preview with multiple templates
- Inline editing and form-based editing
- AI assistance using Google Gemini API
- AI summary and bullet point generation
- Public shareable resume links
- Print and PDF export support
- Strapi backend integration
- MySQL database support through Strapi

---

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Frontend | React, Vite, Tailwind CSS, shadcn/ui |
| Backend | Strapi CMS, REST API |
| Authentication | Clerk |
| Database | MySQL |
| AI Integration | Google Gemini API |
| UI / Utilities | lucide-react, Sonner, Axios |

---

## ⚡ Frontend Setup

Install dependencies:

```bash
npm install
````

Run the frontend development server:

```bash
npm run dev
```

Frontend URL:

```text
http://localhost:5173
```

---

## 🔌 Backend Setup

Go to the backend folder:

```bash
cd backend
```

Install backend dependencies:

```bash
npm install
```

Run Strapi:

```bash
npm run develop
```

Backend URL:

```text
http://localhost:1337
```

---

## ⚙️ Environment Variables

Create a `.env` file in the frontend project and add:

```env
VITE_STRAPI_API_URL=http://localhost:1337
VITE_STRAPI_API_KEY=your_strapi_api_key
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
VITE_GEMINI_API_KEY=your_gemini_api_key
```

> Actual API keys are not included in the repository for security reasons.

---

## 🧪 Demo / Tester Account

A tester account is available for evaluating the Resume Builder system without creating a new account.

| Field    | Details                                                                                                                                                    |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Email    | `resume.tester123@gmail.com`                                                                                                                               |
| Username | `resumeTester`                                                                                                                                             |
| Purpose  | Testing the dashboard, resume editor, templates, live preview, public sharing, print/PDF export, duplicate, archive, publish, restore, and delete features |

<details>
  <summary>Password</summary>

`apple.juice99`

</details>

The tester account includes sample resumes with work experience, education, skills, custom sections, and theme settings so the main system functionality can be tested quickly.

---

## 📁 Project Structure

```text
resume-builder/
├── public/                  # Public static files such as favicon, logo, and images
├── service/                 # API services and helper functions for Strapi requests
├── src/
│   ├── assets/              # Images, icons, and static frontend assets
│   ├── components/          # Reusable React components and UI elements
│   ├── hooks/               # Custom React hooks used across the application
│   ├── lib/                 # Utility functions, constants, and shared helpers
│   ├── pages/               # Main application pages such as Home, Dashboard, Editor, View, and Public Resume
│   └── styles/              # Global CSS files, print styles, and resume styling
├── index.html               # Main HTML file used by Vite to load the React app
├── package.json             # Project dependencies and npm scripts
└── README.md                # Project documentation
```

---

## 📌 Main System Modules

### Authentication

The system uses Clerk for user sign-up, sign-in, email verification, and account session management.

### Dashboard

The dashboard allows authenticated users to manage their resumes. Users can create, search, view, edit, duplicate, publish, archive, restore, and delete resumes.

### Resume Editor

The resume editor allows users to update resume content using guided forms and a live preview. It supports personal details, summary, work experience, education, skills, and custom sections.

### AI Assistance

The system uses Google Gemini API to help users generate and improve resume content, including professional summaries and bullet points.

### Templates and Themes

Users can customize resume appearance using templates and theme settings such as colors, fonts, spacing, and line height.

### Public Sharing and Export

Users can publish resumes, generate public shareable links, and print or export resumes as PDF files.

---

## 🗄️ Database Collections

The Strapi backend manages the following main collections:

* UserResume
* Resume
* Work
* Education
* Skill
* CustomSection
* Theme

---

## 📌 Notes

* The system uses Strapi `documentId` when working with API records and relations.
* Resume data is stored and managed through Strapi.
* Authentication is handled using Clerk.
* AI content generation is handled through Google Gemini API.
* The project supports multiple resumes per user.
* Published resumes can be shared using public read-only links.
* Archived resumes are read-only unless restored.
* Private resume data is only accessible to authenticated users.
* API keys and sensitive environment variables should not be committed to GitHub.

---

## 👩‍💻 Project Information

| Field        | Details                        |
| ------------ | ------------------------------ |
| Project Name | Resume Builder with AI         |
| Student      | Razan Adel Alzari              |
| Student ID   | 6220150                        |
| Course       | TM471 Final Year Project       |
| University   | Arab Open University – Bahrain |

---

## 📄 License

This project was developed as part of a final year university project.

```
```

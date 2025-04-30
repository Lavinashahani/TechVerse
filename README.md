# TechVerse - Technical Blog App

A responsive **technical blogging platform** built using **React**, **Redux**, **Tailwind CSS**, and **Appwrite** (as BaaS). This application allows users to **create**, **read**, **edit**, and **delete** blog posts with user authentication (sign-up & login). Built with **Vite** for fast bundling.

---

## Features

- User authentication (Sign up, Login, Logout)
- Create new blog posts
- Edit and delete existing posts
- View all posts or a single blog article
- Persistent user session using Redux store
- Responsive and clean UI with Tailwind CSS

---

## Tech Stack

| Technology     | Purpose                          |
|----------------|----------------------------------|
| React          | Frontend UI                      |
| Redux Toolkit  | Global state management          |
| Vite           | Lightning-fast bundler           |
| Tailwind CSS   | Utility-first CSS framework      |
| Appwrite       | Backend as a Service (BaaS)      |

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/technical-blog-app.git
cd technical-blog-app

```

### 2. Install Dependencies
Make sure you have Node.js installed.

```bash
npm install
```
### 3. Set Up Tailwind CSS
Tailwind is already configured with Vite. You can customize styles in tailwind.config.js and apply utility classes directly in JSX files.

### 4. Set Up Appwrite
a. Install Appwrite: Installation Guide

b. Create a project in Appwrite dashboard

c. Enable Authentication

d. Create a Database and add a collection named Articles with the following fields:

  -- title (string)

  -- content (string)

  -- authorId (string)

  -- createdAt (datetime)

### 5. Environment Variables
Create a .env file in your project root and add:

```bash
VITE_APPWRITE_ENDPOINT=https://your-appwrite-endpoint/v1
VITE_APPWRITE_PROJECT_ID=your-project-id
VITE_APPWRITE_DATABASE_ID=your-database-id
VITE_APPWRITE_COLLECTION_ID=your-articles-collection-id
```

Replace the placeholders with actual values from your Appwrite dashboard.

### 6. Start the App

```bash
npm run dev
```

Visit: http://localhost:5173

### Folder Structure
```bash
src/
├── app/                # Redux store setup
│   └── store.js
├── components/
│   ├── Auth/
│   ├── Blog/
├── features/           # Redux slices
│   └── authSlice.js
│   └── postSlice.js
├── pages/              # Page components
├── services/           # Appwrite service methods
├── styles/             # Tailwind global styles
├── App.jsx
├── main.jsx
```

### Scripts
  --- npm run dev: Run development server

  --- npm run build: Build for production

  --- npm run preview: Preview the production build


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

## Screenshots

*(Add screenshots of your app here, e.g., login page, dashboard, blog editor, etc.)*

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/technical-blog-app.git
cd technical-blog-app


Set Up Tailwind CSS
Tailwind is already configured with Vite. You can customize styles in tailwind.config.js and apply classes directly in JSX files.

4. Set Up Appwrite
Install Appwrite: Installation Guide

Create a project in Appwrite dashboard

Enable Authentication and create:

A Users system

A Database with a collection for blog posts

Set up the following fields in your Articles collection:

title (string)

content (string or rich text)

authorId (string)

createdAt (datetime)

5. Environment Variables
Create a .env file in the project root:

env
Copy
Edit
VITE_APPWRITE_ENDPOINT=https://your-appwrite-endpoint/v1
VITE_APPWRITE_PROJECT_ID=your-project-id
VITE_APPWRITE_DATABASE_ID=your-database-id
VITE_APPWRITE_COLLECTION_ID=your-articles-collection-id
6. Start the App
bash
Copy
Edit
npm run dev
Open your browser at http://localhost:5173

Folder Structure
plaintext
Copy
Edit
src/
├── app/                # Redux store setup
│   └── store.js
├── components/
│   ├── Auth/
│   ├── Blog/
├── features/           # Redux slices
│   └── authSlice.js
│   └── postSlice.js
├── pages/              # Route pages
├── services/           # Appwrite service methods
├── styles/             # Tailwind base styles
├── App.jsx
├── main.jsx
Scripts
npm run dev: Run development server

npm run build: Build for production

npm run preview: Preview the production build

Contributing
Pull requests are welcome. For major changes, open an issue first to discuss what you’d like to change.

License
This project is licensed under the MIT License.

Contact
For any queries, reach out to [yourname@email.com]

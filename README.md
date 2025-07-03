# 📰 MegaBlog – Full Stack Blogging Platform

**MegaBlog** is a full-stack blog platform built with **React**, **Vite**, and **Appwrite**, allowing users to sign up, write rich content, upload images, and manage blog posts.

> 🚀 Live Demo: [https://megablog-two.vercel.app](https://megablog-two.vercel.app)

---



## ⚙️ Features

- ✅ User authentication (signup, login, logout)
- 📝 Rich text editor with image support
- 🖼️ Upload featured images using Appwrite storage
- ✏️ Create, edit, and delete blog posts
- 🔐 Private routing with Redux
- 🎨 Clean UI using Tailwind CSS

---

## 🛠️ Tech Stack

| Frontend       | Backend / Cloud       |
|----------------|------------------------|
| React + Vite   | Appwrite (Cloud)       |
| React Router   | Appwrite Auth          |
| Tailwind CSS   | Appwrite Database      |
| Redux Toolkit  | Appwrite Storage       |
| React Hook Form|                        |

---

## 📁 Folder Structure

12MegaBlog/
├── 12MegaBlog/             ← actual source root
│   ├── public/             ← static files (favicon, index.html)
│   ├── src/
│   │   ├── appwrite/       ← AppWrite SDK & auth helper
│   │   │   └── auth.js
│   │   ├── components/     ← reusable UI bits
│   │   │   ├── container/  │   Layout helper (Container.jsx)
│   │   │   ├── Footer/     │   Footer.jsx
│   │   │   ├── Header/     │   Header.jsx & LogoutBtn.jsx
│   │   │   └── post-form/  │   PostForm.jsx
│   │   ├── conf/           ← app configuration constants
│   │   │   └── conf.js
│   │   ├── pages/          ← “screens” mapped to routes
│   │   │   ├── Home.jsx
│   │   │   ├── AllPosts.jsx
│   │   │   ├── AddPost.jsx
│   │   │   ├── EditPost.jsx
│   │   │   ├── Post.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Signup.jsx
│   │   ├── store/          ← Redux Toolkit store and slices
│   │   │   ├── store.js    │   configureStore, root reducer
│   │   │   └── authSlice.js│   auth state/actions
│   │   ├── App.jsx         ← root component (layout + auth check)
│   │   ├── App.css         ← global styles (Tailwind + custom)
│   │   └── index.jsx       ← ReactDOM.render + Provider + Router
│   ├── package.json
│   └── vite.config.js

---

## 📦 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/12MegaBlog.git
cd 12MegaBlog
```
### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Appwrite
Update /conf/conf.js with your Appwrite credentials:
```javascript
const conf = {
  appwriteUrl: 'https://cloud.appwrite.io/v1',
  appwriteProjectId: 'your_project_id',
  appwriteDatabaseId: 'your_database_id',
  appwriteCollectionId: 'your_collection_id',
  appwriteBucketId: 'your_bucket_id',
};

export default conf;
```

### 4. Start Development Server
```bash
npm run dev
```
Visit: http://localhost:5173

## 🌐 Deployment (Vercel)

This project is deployed via Vercel.

Install Command: npm install

Build Command: npm run build

Output Directory: dist

Live Site 👉 https://megablog-two.vercel.app
---


## 🙋‍♂️ Author
Made with ❤️ by Venu
🎓 B.Tech CSE | Passionate Web Developer | Aspiring MAANG Engineer
📫 [Connect on LinkedIn](www.linkedin.com/in/
venu-chinthakunta-2544a732a
)
---

## 📄 License
---

This project is open source and free to use under the [MIT License](LICENSE).
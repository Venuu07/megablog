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
├── public/
├── src/
│ ├── appwrite/ # Appwrite SDK and service files
│ │ └── auth.js
│ ├── components/ # UI components
│ │ ├── container/
│ │ ├── Footer/
│ │ ├── Header/
│ │ └── post-form/
│ ├── conf/ # Configuration file
│ │ └── conf.js
│ ├── pages/ # Route-mapped pages
│ │ ├── Home.jsx
│ │ ├── AllPosts.jsx
│ │ ├── AddPost.jsx
│ │ ├── EditPost.jsx
│ │ ├── Post.jsx
│ │ ├── Login.jsx
│ │ └── Signup.jsx
│ ├── store/ # Redux store and slices
│ │ ├── store.js
│ │ └── authSlice.js
│ ├── App.jsx
│ ├── App.css
│ └── main.jsx
├── package.json
├── vite.config.js
└── README.md

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

- Made with ❤️ by Venu
- 🎓 B.Tech CSE | Passionate Web Developer | Aspiring MAANG Engineer
📫 [Connect on LinkedIn](www.linkedin.com/in/
venu-chinthakunta-2544a732a
)
---

## 📄 License

This project is open source and free to use under the [MIT License](LICENSE).
---
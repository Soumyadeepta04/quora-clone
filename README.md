# Quora Clone – Ask, Answer, Engage  
Quora Clone is a responsive web application that mirrors the core features of the original Quora platform. It offers personalized user experiences with account registration and login, enabling users to explore a dynamic feed of community-driven questions, answers, and topic-based discussions.

This web application replicates the core functionalities of Quora — allowing users to ask questions, post answers, upvote/downvote, and browse curated content based on interests.

---

## ✨ Key Features
✅ User Authentication: Register and log in to maintain a personalized experience.

✅ Question & Answer Posting: Users can ask questions and contribute by answering others’ queries.

✅ Upvote/Downvote Mechanism: Community moderation through voting on answers.

✅ Responsive UI/UX: Seamless experience across desktops, tablets, and mobile devices.

✅ Dynamic Home Feed: Real-time feed showcasing trending questions and answers.

✅ Topic-Based Discussions: Explore questions by interest areas.

✅ Search Functionality: Easily find relevant content, questions, or topics with built-in search.
---

## 🛠 Tech Stack  
**Frontend:** React.js, Redux Toolkit  
**Styling:** Custom CSS (quora-style)  
**State Management:** Redux  
**Routing:** React Router  
**(Optional Backend):** Firebase / Express + MongoDB

---

## 📂 Project Structure  

```bash
QUORA-CLONE/
├── .firebase/ # Firebase deployment settings
├── node_modules/ # Installed dependencies
├── public/ # Static assets
├── src/
│ ├── app/ # Redux store configuration
│ ├── components/ # UI components (Header, Sidebar, Feed, etc.)
│ ├── features/ # Redux slices or logic modules
│ ├── App.js # Main app layout
│ ├── App.css # Global styles
│ ├── firebase.js # Firebase config and init
│ ├── index.js # Root render
│ ├── index.css # Base styles
│ └── serviceWorker.js # Optional PWA service worker
├── .eslintrc / .eslintcache # ESLint config/cache
├── .firebaserc # Firebase project alias
├── .gitignore # Git ignored files
├── firebase.json # Firebase deploy rules
├── package-lock.json # NPM lock file
└── package.json # Project metadata
```
 ## Install dependencies
```bash
npm install
```
## 💾Configure Firebase

Create a Firebase project at https://console.firebase.google.com
Then, in src/firebase.js, replace with your config:
```bash
import { initializeApp } from "firebase/app";

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "SENDER_ID",
  appId: "APP_ID",
};

const app = initializeApp(firebaseConfig);
export default app;
```
## ▶️ Run the Projecte Project
```bash
npm start
```
Visit: http://localhost:3000

## 🔥 Deploy to Firebase

### 1. Initialize Firebase
```bash
firebase login
firebase init
```
Choose: Hosting
Select existing Firebase project
Set build or public as hosting directory

### 2.Build and Deploy
```bash
npm run build
firebase deploy
```

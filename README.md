# Instagram Clone

A full-stack Instagram clone application built with modern web technologies, featuring real-time messaging, stories, posts, comments, and user interactions.

## ✨ Features

- 🔐 **Authentication**: JWT-based authentication with Google OAuth
- 📸 **Posts**: Create, edit, delete, and interact with posts
- 💬 **Real-time Messaging**: Socket.io-powered messaging with media support
- 📱 **Stories**: Create and view stories with music support
- 💬 **Comments & Replies**: Interactive comment system
- 👥 **User Profiles**: Follow/unfollow functionality
- 🔔 **Notifications**: Real-time notifications
- 📹 **Video Calls**: Peer-to-peer video calling
- 🎨 **Modern UI**: Responsive design with TailwindCSS and Framer Motion
- ⚡ **Performance**: Optimized with caching and lazy loading

## 🛠 Tech Stack

**Frontend:** Next.js 15, React 19, TypeScript, Redux Toolkit, TailwindCSS, Socket.io, PeerJS

**Backend:** Express.js 5, MongoDB, Socket.io, JWT, Cloudinary, FFmpeg, Twilio

## 📁 Project Structure

This project uses Git Submodules:

```
InstagramClone/
├── front-end/    # Next.js frontend
└── bach-end/     # Express.js backend
```

**Submodules:**
- `front-end`: [InstagramClone_Front-End](https://github.com/vanloc19/InstagramClone_Front-End)
- `bach-end`: [InstagramClone_BackEnd](https://github.com/vanloc19/InstagramClone_BackEnd)

## 🚀 Quick Start

### Prerequisites

- Node.js v18.x or higher
- MongoDB v6.x or higher
- Git

### Installation

```bash
# Clone with submodules
git clone --recurse-submodules git@github.com:vanloc19/InstagramClone.git
cd InstagramClone

# Install backend dependencies
cd bach-end
npm install

# Install frontend dependencies
cd ../front-end
npm install
```

### Running

**Development:**

```bash
# Backend (runs on http://localhost:5000)
cd bach-end
npm run server

# Frontend (runs on http://localhost:3000)
cd front-end
npm run dev
```

**Production:**

```bash
# Build and start frontend
cd front-end
npm run build
npm start

# Start backend
cd bach-end
npm start
```

## 🔧 Submodules

Update submodules to latest version:

```bash
git submodule update --remote
```

## 📝 Notes

- This project uses Git Submodules for frontend and backend
- Initialize submodules when cloning: `git submodule update --init --recursive`
- Each submodule can be developed and deployed independently

## 📄 License

Copyright © 2025 vanloc19. All rights reserved.

This project is proprietary and confidential. Unauthorized copying, modification, distribution, or use of this project, via any medium is strictly prohibited.

## 👤 Contact

**vanloc19**

- 📧 Email: [tovanloc19@gmail.com](mailto:tovanloc19@gmail.com)
- 📘 Facebook: [vanloc1963](https://www.facebook.com/vanloc1963/)
- 💻 GitHub: [@vanloc19](https://github.com/vanloc19)

---

**Note:** This is a clone project for educational purposes. Please comply with Instagram's terms of service and respect intellectual property rights.

# Instagram Clone

A full-stack Instagram clone application built with modern web technologies, featuring real-time messaging, stories, posts, comments, and user interactions.

## 📋 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Project](#running-the-project)
- [Detailed Project Structure](#detailed-project-structure)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

- 🔐 **Authentication & Authorization**: JWT-based authentication with Google OAuth support
- 📸 **Posts Management**: Create, edit, delete, and interact with posts
- 💬 **Real-time Messaging**: Socket.io-powered messaging with media support
- 📱 **Stories**: Create and view stories with music support
- 💬 **Comments & Replies**: Interactive comment system with replies
- 👥 **User Profiles**: Comprehensive user profiles with follow/unfollow functionality
- 🔔 **Notifications**: Real-time notifications for user interactions
- 📹 **Video Calls**: Peer-to-peer video calling functionality
- 🎨 **Modern UI**: Responsive design with TailwindCSS and Framer Motion
- ⚡ **Performance**: Optimized with caching, compression, and lazy loading

## 🛠 Tech Stack

### Frontend
- **Framework**: Next.js 15 (App Router)
- **Language**: TypeScript
- **UI Library**: React 19
- **State Management**: Redux Toolkit, Zustand
- **Styling**: TailwindCSS, SCSS
- **Animation**: Framer Motion
- **Real-time**: Socket.io Client
- **Data Fetching**: SWR
- **Video Calls**: PeerJS

### Backend
- **Framework**: Express.js 5
- **Database**: MongoDB (Mongoose)
- **Authentication**: JWT, Google OAuth
- **Real-time**: Socket.io
- **File Upload**: Cloudinary, Multer
- **Security**: Helmet, CORS, bcrypt
- **Caching**: API Cache
- **Video Processing**: FFmpeg
- **Communication**: Twilio (for calls)

## 📁 Project Structure

This project uses Git Submodules to manage the frontend and backend repositories:

```
InstagramClone/
├── front-end/          # Frontend submodule (Next.js)
├── bach-end/           # Backend submodule (Express.js)
└── README.md           # This file
```

### Submodules
- **front-end**: `git@github.com:vanloc19/InstagramClone_Front-End.git` (branch: main)
- **bach-end**: `git@github.com:vanloc19/InstagramClone_BackEnd.git` (branch: main)

## 📦 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js**: v18.x or higher
- **npm**: v9.x or higher (or yarn/pnpm)
- **MongoDB**: v6.x or higher (local or Atlas)
- **Git**: Latest version
- **FFmpeg**: For video processing (backend)

## 🚀 Installation

### 1. Clone the Repository

Clone this repository along with its submodules:

```bash
# Clone with submodules
git clone --recurse-submodules git@github.com:vanloc19/InstagramClone.git

# Or if you've already cloned without submodules
git submodule update --init --recursive
```

### 2. Install Dependencies

Install dependencies for both frontend and backend:

```bash
# Install backend dependencies
cd bach-end
npm install

# Install frontend dependencies
cd ../front-end
npm install
```

## 🏃 Running the Project

### Development Mode

#### Start Backend Server

```bash
cd bach-end
npm run server
```

The backend server will run on `http://localhost:5000`

#### Start Frontend Server

```bash
cd front-end
npm run dev
```

The frontend will run on `http://localhost:3000`

### Production Mode

#### Build Frontend

```bash
cd front-end
npm run build
npm start
```

#### Start Backend

```bash
cd bach-end
npm start
```

## 📂 Detailed Project Structure

### Backend (`bach-end/`)
```
bach-end/
├── config/              # Configuration files
│   ├── db.config.js    # MongoDB configuration
│   └── cloudinary.config.js
├── controllers/         # Route controllers
├── middlewares/         # Custom middlewares
├── models/              # Mongoose models
├── routes/              # API routes
├── server/              # Socket.io services
├── utils/               # Utility functions
├── helper/              # Helper functions
└── app.js              # Main application file
```

### Frontend (`front-end/`)
```
front-end/
├── src/
│   ├── app/            # Next.js App Router pages
│   ├── components/     # React components
│   ├── contexts/       # React contexts
│   ├── hooks/          # Custom hooks
│   ├── server/         # Server-side utilities
│   ├── store/          # Redux store
│   ├── types/          # TypeScript types
│   └── utils/          # Utility functions
└── public/             # Static assets
```

## 📚 API Documentation

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user
- `POST /api/auth/logout` - Logout user
- `GET /api/auth/me` - Get current user

### Posts
- `GET /api/posts` - Get all posts
- `POST /api/posts` - Create new post
- `GET /api/posts/:id` - Get post by ID
- `PUT /api/posts/:id` - Update post
- `DELETE /api/posts/:id` - Delete post
- `POST /api/posts/:id/like` - Like/unlike post

### Users
- `GET /api/users/:id` - Get user profile
- `PUT /api/users/:id` - Update user profile
- `POST /api/users/:id/follow` - Follow user
- `POST /api/users/:id/unfollow` - Unfollow user

### Messaging
- `GET /api/messenger/conversations` - Get conversations
- `GET /api/messenger/messages/:conversationId` - Get messages
- `POST /api/messenger/send` - Send message

### Stories
- `GET /api/stories` - Get all stories
- `POST /api/stories` - Create story
- `GET /api/stories/:id` - Get story by ID

## 🔧 Updating Submodules

If you need to update the submodules to their latest versions:

```bash
# Update all submodules
git submodule update --remote

# Update specific submodule
git submodule update --remote front-end
git submodule update --remote bach-end
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Notes

- This project uses Git Submodules to manage separate repositories for frontend and backend
- Make sure to initialize and update submodules when cloning the repository
- Each submodule can be developed and deployed independently

## 📄 License

This project is licensed under the ISC License.

## 👤 Author

**vanloc19**

- GitHub: [@vanloc19](https://github.com/vanloc19)

## 🙏 Acknowledgments

- Inspired by Instagram's functionality and user experience
- Built with modern web technologies and best practices

---

**Note**: This is a clone project for educational purposes. Make sure to comply with Instagram's terms of service and respect intellectual property rights.


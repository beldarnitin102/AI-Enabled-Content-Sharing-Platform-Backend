# Akatsuki's Draft – AI-Enabled Content Sharing Platform (Backend)

**Nodevember 4.0 · Node.js · Express · MongoDB (Mongoose) · JWT · Google Gemini**

🚀 **Live Deployment:** [View Live API / App](https://ai-enabled-content-sharing-platform.onrender.com)

## Setup

```bash
npm install
cp .env.example .env     # fill in MONGO_URI, JWT_SECRET, GEMINI_API_KEY, ADMIN_SECRET
npm run dev              # or: npm start
Requires Node 18+ and a running MongoDB (local or Atlas).

Folder structure
Plaintext
server.js
src/
  app.js              express app + routes
  config/db.js        mongoose connection
  models/             User, Post
  middleware/         auth (JWT + admin), error, validateId, upload
  controllers/        auth, post, admin, ai
  routes/             auth, posts, admin, ai
  services/gemini.js  Gemini integration

# Talent Hub

A simple Node.js application that allows users to register, log in, post job listings, and apply for jobs. The app uses Express, EJS templates, and a tiny JSON file for data persistence, so no external database or Docker is required.

## Features
- User registration & login (bcrypt password hashing, session management)
- Dashboard for viewing posted jobs and applications
- Create, view, and apply to job listings
- Simple JSON‑file based storage (`data.json`)
- Clean UI built with EJS and a small CSS stylesheet

## Project Structure
```
TalentHub/
├─ public/
│  └─ css/style.css
├─ views/
│  ├─ index.ejs
│  ├─ register.ejs
│  ├─ login.ejs
│  ├─ dashboard.ejs
│  ├─ jobs.ejs
│  ├─ post-job.ejs
│  ├─ job-detail.ejs
│  └─ 404.ejs
├─ db.js                # Simple JSON DB helper
├─ server.js            # Main Express app
├─ package.json
├─ package-lock.json
└─ README.md
```

## Setup & Run
1. **Clone the repository** (if you haven't already):
   ```bash
   git clone https://github.com/Krish-119/repo_nodejs.git
   cd repo_nodejs
   ```
2. **Install dependencies**:
   ```bash
   npm install
   ```
3. **Start the server**:
   ```bash
   npm start
   ```
   The app will be available at `http://localhost:3000`.

## Scripts
- `npm start` – Runs `node server.js`.
- `npm run dev` – (optional) start with `nodemon` if you have it installed.

## notes
- The app stores data in `data.json` created automatically on first use. You may want to add this file to `.gitignore` if you don't want to commit user data.
- If port **3000** is already in use, stop the other process or change the port in `server.js`.

## License
This project is provided as a learning/example project and is free to use.

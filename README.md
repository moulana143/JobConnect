# JobConnect – Job Portal Application

A responsive student project built with HTML, CSS, JavaScript, Node.js and Express.

## Features
- Job seeker and employer registration/login
- Job listing, keyword/location/type search
- Save and apply for jobs
- Application tracking and employer status updates
- Employer job posting and applicant review
- Keyword-based job alerts
- Resume builder with downloadable text resume
- Mobile-friendly interface and sample job listings

## Run locally
1. Install Node.js 18 or later.
2. Extract this ZIP.
3. Open a terminal in this folder.
4. Run `npm install`
5. Run `npm start`
6. Open `http://localhost:3000`

The server creates `data/db.json` automatically.

## Upload to GitHub
Extract this ZIP on your phone/computer. Upload the **contents** of the `JobConnect_Project` folder to the root of your GitHub repository. Do not upload only the ZIP file.

## Deploy on Render
1. Connect your GitHub repository to Render as a Web Service.
2. Build command: `npm install`
3. Start command: `npm start`
4. Set environment variable `DATA_DIR` to `/var/data`.
5. Add a persistent disk mounted at `/var/data` to keep the JSON database across restarts.

## Project limitations
This is an educational demo, not a production hiring service. Session tokens are kept in server memory and will expire when the server restarts. Job alerts are stored keywords only; email/SMS notifications are not configured. Resume drafts are stored in the browser on that device. Do not use real sensitive personal data in a public demo. Add persistent sessions, stronger security, validation, privacy controls and backups before production use.

## Structure
- `server.js` – Express backend and API
- `package.json` – dependencies and start script
- `public/index.html` – app page
- `public/style.css` – responsive design
- `public/app.js` – front-end features
- `render.yaml` – optional Render deployment blueprint
- `.env.example` – environment examples

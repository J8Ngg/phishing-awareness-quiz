# Phishing Awareness Quiz (Science Fair Project)

**Live Demo:** https://j8ngg.github.io/phishing-awareness-quiz/

An interactive, browser-based phishing awareness quiz designed for K–12 students.

## What it does
- Shows 5 randomized “email” scenarios pulled from a larger question bank
- Lets players classify each as **Legitimate** or **Phishing**
- Provides explanations and a one-time “red flags” educational popup for missed phishing questions
- Tracks a local leaderboard using browser `localStorage`

## Run locally
### Option A: Python web server (recommended)
1. Find your machine IP:
   - Linux/macOS: `ip a` (or `ifconfig`)
   - Windows: `ipconfig`
2. Start a local server:
   ```bash
   python -m http.server --bind <YOUR_IP> 1337
   ```
3. Open in a browser:
   - `http://<YOUR_IP>:1337/`

### Option B: Just open the file
You *can* double-click `index.html`, but some browsers are stricter about local file behavior. The local server is more reliable.

## Deploy on GitHub Pages
1. Create a new GitHub repo (example: `phishing-awareness-quiz`)
2. Upload these files to the repo root:
   - `index.html`
   - `knight-logo.png`
3. In the repo: **Settings → Pages**
   - Source: **Deploy from a branch**
   - Branch: `main`
   - Folder: `/ (root)`
4. GitHub will give you a public URL (your live demo link).

## Notes
- The leaderboard is **per-device** (saved in the browser), not a shared online leaderboard.
- This project is for awareness/education—no real credential collection.

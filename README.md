# Akshai Narayanappa — Portfolio

A personal portfolio website built with React, featuring an AI-powered resume summarizer powered by the Anthropic Claude API.

## 🔗 Live Demo
> Coming soon — [deploy to Vercel or GitHub Pages]

---

## ✨ Features

- **Hero section** — Name, role, and quick intro
- **Skills & Tech Stack** — Python, SQL, GCP, BigQuery, Airflow, and more
- **Work Experience** — Timeline of roles and responsibilities
- **Projects** — Showcase of key data engineering work
- **AI Resume Summarizer** — Click a button and Claude generates a live professional summary of the resume
- **Contact** — Email and location info

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React |
| AI | Anthropic Claude API (`claude-sonnet-4`) |
| Styling | Inline CSS with CSS variables |
| Deployment | Vercel / GitHub Pages |

---

## 🚀 Getting Started

### Prerequisites
- Node.js v18+
- npm or yarn
- Anthropic API key → [console.anthropic.com](https://console.anthropic.com)

### Installation

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/akshai-portfolio.git
cd akshai-portfolio

# Install dependencies
npm install

# Start the dev server
npm start
```

### Environment Variables

Create a `.env` file in the root:

```env
REACT_APP_ANTHROPIC_API_KEY=your_api_key_here
```

Then update the fetch call in `App.js` to use:
```js
headers: {
  "Content-Type": "application/json",
  "x-api-key": process.env.REACT_APP_ANTHROPIC_API_KEY,
  "anthropic-version": "2023-06-01"
}
```

> ⚠️ **Note:** Never commit your API key to GitHub. The `.env` file is listed in `.gitignore` by default in Create React App.

---

## 📁 Project Structure

```
akshai-portfolio/
├── public/
│   └── index.html
├── src/
│   ├── App.js          # Main portfolio component
│   └── index.js        # React entry point
├── .env                # API keys (not committed)
├── .gitignore
├── package.json
└── README.md
```

---

## 📦 Deployment

### Vercel (recommended)
1. Push repo to GitHub
2. Import at [vercel.com](https://vercel.com)
3. Add `REACT_APP_ANTHROPIC_API_KEY` in Vercel's Environment Variables
4. Deploy — done!

### GitHub Pages
```bash
npm install gh-pages
```
Add to `package.json`:
```json
"homepage": "https://YOUR_USERNAME.github.io/akshai-portfolio",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
```
```bash
npm run deploy
```

---

## 👤 About Me

**Akshai Narayanappa** — Data Engineer at Prodapt Solutions, Bangalore.
3+ years of experience in Python, SQL, BigQuery, GCP, and Airflow.

- 📧 akshai.narayanappa@gmail.com
- 🏙️ Bangalore, India

---

## 📄 License

MIT License — feel free to use this as a template for your own portfolio.
```

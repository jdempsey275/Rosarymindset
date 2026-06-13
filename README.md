# Rosary Mindset

An online OCIA course that allows people to learn the Catholic faith at their own pace, with a required parish sponsor relationship woven into the experience.

## Features

- **Full OCIA curriculum** — 8 sections covering Inquiry, Scripture & Tradition, The Creed, Prayer & Liturgy, The Sacraments, Moral Life, The Church, and Mystagogy
- **Login system** — user authentication with progress saved to localStorage
- **Parish sponsor** — sponsor info displayed throughout; required meetings gate course progression
- **3 required sponsor meetings** — locked checkpoints ensure pastoral accompaniment
- **Personal reflection journal** — each section has written reflection prompts before advancing
- **Progress tracking** — animated candle that fills as sections are completed
- **Fully responsive** — works on desktop and mobile

## Deployment to Vercel

### Option 1 — From GitHub (recommended)

1. Push this folder to a GitHub repository
2. Go to [vercel.com](https://vercel.com) and click **Add New Project**
3. Import your GitHub repo
4. Vercel will detect the static site automatically — no build step needed
5. Click **Deploy**

### Option 2 — Vercel CLI

```bash
npm i -g vercel
cd rosary-mindset
vercel
```

## Managing Users

In `index.html`, find the `USERS` object near the top of the `<script>` tag:

```javascript
const USERS = {
  'username': { password: 'password', name: 'Full Name', initials: 'FN', display: 'First N.' }
};
```

Add or update entries to create accounts for each learner.

## Customizing the Sponsor

Search for `Michael Flanagan` in `index.html` to update the sponsor name, phone, email, and parish.

## File Structure

```
rosary-mindset/
  index.html    ← entire app (HTML + CSS + JS, single file)
  vercel.json   ← Vercel routing config
  README.md     ← this file
```

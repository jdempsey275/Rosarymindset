# The Journey — OCIA Online

An online course that teaches the full OCIA (Order of Christian Initiation of Adults) curriculum, allowing people to learn the Catholic faith at their own pace while maintaining a parish sponsor relationship.

## Features

- **Full OCIA curriculum** — 8 sections covering Inquiry, Scripture & Tradition, The Creed, Prayer & Liturgy, The Sacraments, Moral Life, The Church, and Mystagogy
- **Login system** — secure user authentication with progress saved to localStorage
- **Parish sponsor** — sponsor info displayed throughout; required meetings gate course progression
- **3 required sponsor meetings** — locked checkpoints ensure pastoral accompaniment
- **Personal reflection journal** — each section has written reflection prompts before you can advance
- **Progress tracking** — animated candle that fills as sections are completed
- **Fully responsive** — works on desktop and mobile

## Login Credentials

| Username | Password |
|----------|----------|
| `journey` | `faith2024` |

## Deployment to Vercel

### Option 1 — From GitHub (recommended)

1. Push this folder to a GitHub repository
2. Go to [vercel.com](https://vercel.com) and click **Add New Project**
3. Import your GitHub repo
4. Vercel will detect the static site automatically
5. Click **Deploy** — done!

### Option 2 — Vercel CLI

```bash
npm i -g vercel
cd ocia-course
vercel
```

## Adding More Users

In `index.html`, find the `USERS` object near the top of the `<script>` tag and add entries:

```javascript
const USERS = {
  'journey': { password: 'faith2024', name: 'Johanna Dempsey', initials: 'JD', display: 'Johanna D.' },
  'newuser': { password: 'theirpassword', name: 'First Last', initials: 'FL', display: 'First L.' }
};
```

## Customizing the Sponsor

Search for `Michael Flanagan` in `index.html` to update sponsor name, phone, email, and parish.

## Structure

```
ocia-course/
  index.html    ← entire app (HTML + CSS + JS, single file)
  vercel.json   ← Vercel routing config
  README.md     ← this file
```

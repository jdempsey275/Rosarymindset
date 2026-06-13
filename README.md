# Rosary Mindset

An online OCIA course with admin account management.

## Logging In

### Learner login
Users go to the main URL and sign in with their username and password.

### Admin login
Click the small **"Admin access →"** link at the bottom of the login card.
Enter the admin password (default: `rosaryadmin2024`).

**Change the admin password** before going live — open `index.html`, find:
```
const ADMIN_PASSWORD = 'rosaryadmin2024';
```
and replace with your own password.

## Admin Panel Features
- **Create accounts** — enter a full name, username, and password for each new learner
- **View all accounts** — see every user and their section progress at a glance
- **Remove accounts** — delete a learner and their progress data

Accounts created in the admin panel are stored in the browser's localStorage on whatever device you use to administer the site.

## Built-in Account (your demo account)
| Username | Password |
|----------|----------|
| `journey` | `faith2024` |

## Deploy to Vercel
1. Create a GitHub repo and upload all three files
2. Go to vercel.com → Add New Project → Import repo → Deploy

## Customizing the Sponsor
Search `index.html` for `Michael Flanagan` to update the sponsor's name, phone, email, and parish.

## Color Palette
- Deep Evergreen `#183A2A`
- Old Gold `#B8945E`
- Warm Cream `#FBF8F2`
- Bronze `#8B6A44`
- Charcoal `#2A2A2A`

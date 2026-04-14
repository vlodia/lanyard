# Lanyard by Vlodia

[![Website](https://img.shields.io/badge/Website-live-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://lanyard.vlodia.com)
[![Organization](https://img.shields.io/badge/Org-vlodia-111214?style=for-the-badge&logo=github&logoColor=white)](https://github.com/vlodia)

**Live site:** [lanyard.vlodia.com](https://lanyard.vlodia.com)

Lanyard is a **product website** that shows a Discord profile as a card: avatar, banner, badges, status, activities, and (if you choose) linked accounts. This README explains **how to use the site**, not how to run or ship source code.

---

## How to use the site

### 1) Open a Discord profile

- Go to [lanyard.vlodia.com](https://lanyard.vlodia.com) in your browser.
- Enter a **Discord user ID** in the field on the home page to open their card. (Enable Developer Mode in Discord → User Settings → Advanced, then right‑click a user → Copy User ID.)
- Profile URLs look like:  
  `https://lanyard.vlodia.com/user/<USER_ID>`  
  Share that link to open someone’s card directly.

**What everyone sees (no login required):** the public profile view—badges, status, activities, Spotify, etc.—based on what the service can resolve from Discord. You cannot see another person’s private linked-accounts list.

### 2) Sign in with Discord (your own account)

- Click **Sign in with Discord** in the header. Discord’s authorization screen opens.
- After you approve, the site sends you to **your own profile page**.
- Signing in lets the site read **your** Discord “connections” (GitHub, Steam, etc.) and show them on **your** card only. Other users’ connections are never exposed to you.

**Sign out:** use the site’s logout flow so your session cookie is cleared.

### 3) When you see the “full” card

- Any user ID can show the base card and presence.
- Extra fields that come from OAuth (such as **connections**) only merge in a meaningful way when **you are signed in** and the page you are viewing is **your own** user ID. On someone else’s profile, that private data is not shown to you.

---

## Privacy and security (short)

- Sign-in uses Discord’s standard OAuth screen; the app only requests the scopes you approve.
- Sessions are handled with a secure cookie on the site and cleared on logout.
- Bot and backend **source code are not distributed** through this repo; it exists for product context and end‑user guidance only.

---

## If something goes wrong

- **Profile missing or empty:** Check that the ID is valid (a 17–19 digit snowflake). If Discord cannot resolve the user, the card may be limited.
- **Sign-in errors:** OAuth and redirects are aligned with the **live site** only. Always start sign-in from [lanyard.vlodia.com](https://lanyard.vlodia.com).
- **Connections not listed:** They only apply on **your** profile while signed in; connections you hide in Discord are not listed here either.

---

## License

This repository contains **documentation only** (this README). The text is licensed under **Creative Commons Attribution 4.0 International** ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).

You may share and adapt the material for any purpose, including commercially, as long as you **give appropriate credit**, provide a link to the license, and indicate if you made changes. See the [full legal text](https://creativecommons.org/licenses/by/4.0/legalcode).

---

## Vlodia

[Lanyard](https://lanyard.vlodia.com) · [Vlodia on GitHub](https://github.com/vlodia)

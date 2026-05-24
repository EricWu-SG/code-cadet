# 🚀 Code Cadet: Galaxy Builder

> A vibe coding learning app — built for my son **Ethan** to learn how to talk to AI and build things.

**🪐 Meet Pixel** — a friendly alien from Planet Codeon who crashed on Earth. To get home, Pixel needs Ethan to teach him how Earth kids talk to AI. Every lesson brings Pixel closer to his family.

---

## What this is

A single-file HTML Progressive Web App that:
- Teaches kids (10+) how to write effective prompts for Claude
- Walks them through building real webpages with AI in 3-step missions
- Tracks streaks, unlocks Hero Cards (Ada Lovelace, Margaret Hamilton, Grace Hopper…), saves progress
- Backs up to email so progress is never lost

## Tech

- **Pure HTML/CSS/JS** — one `index.html`, no build step
- **PWA** — `manifest.json` + service worker for offline support
- **localStorage** — saves all progress on device
- **mailto: backup** — daily progress email to parent

## Curriculum (6 weeks)

| Week | Theme | Status |
|------|-------|--------|
| 1 | First Contact — Hello, AI Builder | ✅ Complete |
| 2 | Prompt Forge — Power of Words | ✅ Complete |
| 3 | Worlds of Wonder — Interest-Driven Builds | 🚧 Skeleton only |
| 4-6 | ??? Mystery worlds | 🔒 Unlocks after Week 3 |

## Deployment

This repo is deployed via **Netlify** with auto-deploy on push to `main`.
See [`docs/PWA_DEPLOY_NOTES.md`](docs/PWA_DEPLOY_NOTES.md) for details.

## Parent dashboard

- Tap the Code Cadet logo (top-left) **5 times quickly**
- Password: configured in `index.html` (`PARENT_PASSWORD`)

---

*Made with ❤️ by Dad. Powered by Claude.*

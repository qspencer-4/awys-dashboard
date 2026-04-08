# AWYS Decision Log

## 2026-04-08: InVideo style — stock footage, not animation
- **Decision:** Stop pushing animated/illustrated character videos
- **Why:** InVideo Basic ($25/mo) does stock footage + text overlays, not custom animation. Animated direction was producing bad results.
- **Impact:** All InVideo prompts and scripts optimize for stock footage cuts, bold text, dynamic transitions

## 2026-04-08: Emojis allowed in social captions
- **Decision:** Emojis OK in YouTube/TikTok/IG/FB captions, NOT in dashboard UI or InVideo prompts
- **Why:** Emojis boost engagement on social platforms. The "no emojis" rule in CLAUDE.md applies to app UI and video text only.

## 2026-04-08: Single HTML file architecture
- **Decision:** Keep dashboard as a single HTML file with vanilla JS
- **Why:** Simple deployment via GitHub Pages, no build tools needed. Solo developer — complexity is the enemy.

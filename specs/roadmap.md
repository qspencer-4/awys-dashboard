# AWYS Roadmap

## Current Priorities (as of 2026-04-08)

### 1. Finish and Test Scraper
- Status: Updated with broad AI trend tracking + category classification
- Test all 4 sources: Reddit, Bing News, YouTube, HackerNews
- Verify /trends/live returns categorized data

### 2. Update Dashboard Generate Tab
- Add category badges next to each trend
- Add category filter row above trends list
- Categories: Make Money, Productivity, Tool Review, AI News, Comparison, Shocking, Beginner

### 3. Fix InVideo Prompt
- Optimize for stock footage + text overlays (Basic plan)
- Strong metaphoric framing without requiring animation
- Each script should suggest visual scenes InVideo can execute with stock

### 4. Wire Scraper into Script Generator
- /generate-script should pull top 5 live trends as context
- Claude knows what's trending when generating scripts

## Completed
- Live trend scraper (Reddit, Bing News, YouTube, HN)
- Category classification in scraper
- Script generator with metaphoric character system
- Dashboard rebuilt: 4 tabs (Generate, Queue, Analytics, Settings)
- Permanent Cloudflare tunnel
- YouTube OAuth connected
- Settings backup/restore via VPS
- Queue tab with platform caption cards + countdown timers
- Deploy button (VPS -> GitHub)

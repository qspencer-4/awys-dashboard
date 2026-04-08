# AWYS Architecture

## Overview
AI While You Sleeping is an AI content automation platform for short-form video.

## Components

### VPS Backend (187.124.240.101)
- **server.py** — Flask app with endpoints: /generate-script, /trends/live, YouTube OAuth
- **scraper.py** — Hits Reddit, Bing News, YouTube, Hacker News for AI trends
- **start.sh** — Startup script for Flask + scraper
- **Cloudflare Tunnel** — Permanent domain at api.aiwhileyousleeping.com

### Dashboard (GitHub Pages)
- **awys-dashboard.html** — Single HTML file, vanilla JS, localStorage
- **Tabs:** Generate, Queue, Analytics, Settings
- **Hosted at:** qspencer-4.github.io/awys-dashboard/
- **Deployed via:** VPS deploy button (pushes from /root/awys/awys-dashboard.html)

### Content Pipeline
- Scraper finds trends -> User picks trend -> Claude API generates script -> InVideo makes video -> Upload to platforms
- Script format: Hook (0-3s), Problem (3-10s), Solution (10-20s), Wow (20-27s), CTA (27-30s)
- Max 80 words, 30 seconds, stock footage style (InVideo Basic)

## Key Constraints
- Single HTML file for dashboard (no build tools)
- One <script> block only (duplicates cause raw JS rendering)
- localStorage for state (domain-specific, use Restore from Server for recovery)
- InVideo Basic plan = stock footage + text overlays, NOT animation

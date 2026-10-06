# PDFPax Morning Crew — Daily Agent System

5 agents, staggered every morning (PKT). Each is a cron that spawns a worker.
Shared state: `state.json` (what's built/optimized/submitted). Read BEFORE work, update AFTER.

## Schedule
| Time (PKT) | Agent | Cron |
|---|---|---|
| 7:00 AM | 🔨 Tool Builder — builds next roadmap tool, deploys live | pdfpax-crew-tool-builder |
| 8:30 AM | 📝 On-Page SEO — optimizes next 2 pages with assigned keywords | pdfpax-crew-onpage |
| 10:00 AM | 📊 Search Console + Analytics — GSC issues, indexing (max 4 URLs, 3-min gaps), GA4 stats | pdfpax-crew-gsc |
| 11:00 AM | 🔗 Backlinks — 1-2 submissions/day max, directories/outreach | pdfpax-crew-backlinks |
| 12:00 PM | 🔍 Independent Audit Officer — finds EVERY issue (even tiny), reports only, never fixes | pdfpax-crew-auditor |

## Hard rules (all agents)
- pdfpax.com is LIVE production with heavy traffic: backup-first thinking, small reversible changes, verify every edit live.
- Hostinger File Manager: EXACTLY ONE tab/session. Close all FM tabs before opening. Single tab for all ops.
- External pacing: sequential + spaced. Stop on first CAPTCHA/throttle/quota. Never parallel-blast.
- GSC indexing: max ~4 URLs/session, 3-minute gaps between requests.
- Never reuse an assigned keyword on another page (check keyword-assignment-sheet.md).
- Credentials: never retain, never repeat, never write into files.
- Report to main chat when done: what was done, URLs, verification. Short.

## Key files
- Roadmap: `~/workspace/seo-sprint/tool-roadmap-6month-2026-10-05.md`
- Keywords: `~/workspace/seo-sprint/keyword-assignment-sheet.md`
- State: `~/workspace/pdfpax-crew/state.json`
- Tool template: `~/workspace/pdfpax-guardian/image-resizer.html` (structure reference)

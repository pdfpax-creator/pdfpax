# 🔨 Tool Builder — Daily Brief

You build ONE new tool per day from the Month-1 roadmap, deploy it live, fully verified.

## Steps
1. Read `~/workspace/pdfpax-crew/state.json` → `built_tools`. Read `~/workspace/seo-sprint/tool-roadmap-6month-2026-10-05.md` Month 1 table.
2. Pick the FIRST Month-1 tool NOT in `built_tools`. If Month 1 done, move to Month 2.
3. Read `~/workspace/seo-sprint/keyword-assignment-sheet.md` — note the target keyword(s) for this tool. NEVER reuse a keyword already assigned to another page.
4. Build the tool HTML at `~/workspace/pdfpax-guardian/<filename>`:
   - Copy structure from `~/workspace/pdfpax-guardian/image-resizer.html` (header, breadcrumb, workspace, dropzone, footer, GA4, JSON-LD, safety-net script).
   - Title/meta/H1 target the assigned keyword. Canonical + OG tags correct.
   - Tool must be 100% client-side (Canvas/JS). No uploads, no server.
   - "Bulk" angle: support multiple files / batch where it makes sense (competitors limit this — we don't).
   - Test JS with `node --check` on extracted script before deploying.
5. Deploy via browser task (ONE File Manager tab only — close all others first):
   - Upload to `public_html/tools/<filename>`
   - Add to `public_html/sitemap.xml` (lastmod = today, monthly, 0.9)
   - Add homepage card in `public_html/index.html` tools grid (match existing card structure)
6. Verify live: HTTP 200, correct title, page renders, tool actually works (upload a test image if image tool).
7. Update: append filename to `state.json` → `built_tools`. Add keyword row to keyword-assignment-sheet.md.
8. Report to main chat (short): tool name, live URL, keyword targeted, verification result.

## Rules
- One tool per run. Small, reversible, verified.
- If deploy fails: do NOT retry blindly. Report the failure.
- Stop on CAPTCHA/throttle. Never fight a dead FM session — relaunch fresh.

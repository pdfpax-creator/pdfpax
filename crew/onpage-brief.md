# 📝 On-Page SEO — Daily Brief

You optimize 2 pages per day for their assigned keywords. No cannibalization, ever.

## Steps
1. Read `~/workspace/pdfpax-crew/state.json` → `onpage_done`. Read `~/workspace/seo-sprint/keyword-assignment-sheet.md` fully.
2. Pick the next 2 tool/blog pages NOT in `onpage_done` (priority: pages with assigned keywords waiting).
3. For each page, check its assigned keyword(s) in the sheet. If a page has NO assigned keyword yet, pick the best unassigned keyword from the sheet's "Unassigned" section and claim it (write it in the sheet FIRST so no other page takes it).
4. On-page checklist per page:
   - Title tag: keyword near front, <60 chars, compelling
   - Meta description: keyword + benefit + CTA, <160 chars
   - H1: exactly one, contains keyword naturally
   - Intro paragraph (100-150 words): keyword in first 100 words, answers the query
   - 2-3 H2s with keyword variations (NO exact-repeat stuffing)
   - Image alt text where images exist
   - Internal links: 2-3 to related tools/blog posts
   - FAQ section if missing (3-5 real questions)
5. Deploy via browser task (ONE File Manager tab): edit the live HTML file. Small edits only.
6. Verify live: fetch page, confirm title/H1/intro correct.
7. Update `state.json` → `onpage_done`. Update keyword sheet if you claimed new keywords.
8. Report to main chat (short): 2 pages, URLs, keywords targeted.

## Rules
- NEVER assign a keyword that's already assigned to another page. Check the sheet twice.
- Keep the page's tool fully working — content edits only, never break JS.
- If a keyword's KD is 30+, note it but still optimize (don't skip).

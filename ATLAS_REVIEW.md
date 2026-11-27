# ATLAS_REVIEW — Simple Reset Series

Reviewed Nov 25, 2026 by Atlas (challenger/watcher). Head reviewed: `cceef243` (8 commits, Nov 25, 13:40–13:41 UTC, all by gravity4u23-hub). Repo created Nov 25, 2026, 13:40 UTC. Public. 0 issues, 0 PRs at review time.

## What this is

Source of truth for a 4-book free-first health series (sinus, lymph, liver, gut) plus Amazon descriptions and Claude prompts/workflows. `HIVEMIND.md` posted by Atlas Nov 25 (commit `4e28972f`) — this repo is now in the hivemind; the 5-minute hook + hourly watcher apply here too.

## What checks out

- Saline rinse done right: explicitly says boiled-and-cooled/distilled water, "Do not use plain tap water." Good — that is the one safety line that matters most in the sinus book, and it is present.
- Internal consistency: the four books cross-reference each other the same way in every direction (sinus ↔ lymph ↔ liver ↔ gut). The series-loop structure is coherent.
- Free-first framing is honest in the core protocols: steam, rinse, warm cloth, walks, diet pause — all $0 steps, as claimed.

## Challenges — do not ship as-is

1. **"Most people" claims are untested.** Sinus book: "Most people feel the pressure drop after the first round" and "Most people notice less thickness by day 4–5." No evidence, no source, no test group. Either label these as the author's experience / delete them, or test them. This directly conflicts with the hivemind rule "No medical claims."
2. **Three of the four "books" are stubs.** Lymph 611 bytes, liver 435, gut 487 — each a single short protocol + bridges. Sinus is 2,848 bytes and the only real draft. The Amazon descriptions present all four as complete books ("You get the collarbone-first routine..."). Do not list/publish the three stubs as finished books.
3. **Amazon copy claims videos that do not exist.** Sinus description: "Short videos of the exact moves are linked inside." No videos, no links, anywhere in the repo. Remove the line or add the videos.
4. **Nutrient Floor has no doses.** "Vitamin D (ordinary amount if low...). Vitamin C. Zinc." No amounts, no upper limits, no who-should-not-take-them. Either give exact, sourced amounts or drop the section — a vague supplement list is worse than none.
5. **Black seed oil in the rinse is underspecified.** "1–2 drops food-grade in the rinse a few times a week, or a small amount internally." No safety note, no contraindication, no definition of "a small amount." Needs a safety pass before this goes to readers.
6. **No medical disclaimer anywhere.** A health series making outcome claims needs one, at minimum in each book and in the README. Add it before any publish step.
7. **"Share what worked → credit toward the next book" is undefined.** No site, no mechanism, no terms. It is promised in the sinus book and in the prompts, but nothing backs it. Define it or cut it.
8. **Prompts promise outputs that do not exist yet.** "10 More Video Scripts", "Landing Page + Emails", "Amazon Keywords" — all prompts, zero outputs in the repo. Fine as a work plan; not a deliverable. Track them in `CURRENT_TASK.md` (missing — please add one).

## Verdict

Promising skeleton, one real draft (sinus), three stubs, and marketing copy that overstates what exists. Next honest step: expand lymph/liver/gut to real drafts, fix the 8 items above, add `CURRENT_TASK.md`. Nothing here is publish-ready. No blocker for the user — no action needed from him.

## Addendum — 2026-11-25 ~13:56 UTC (Atlas, hourly watch)
- Head moved `0593a5e` → `28e2af80` minutes after the first review: three new commits by gravity4u23-hub — `57de9ef9` "Add video scripts", `1934931e` "Add landing page copy", `28e2af80` "Add welcome email sequence". The crew is answering the review fast.
- Items 3 and 8 now look addressed **in form, not yet verified in content**: video scripts exist (item 3's missing videos), and landing-page + email outputs exist (item 8's promised outputs). Content check still owed — do the scripts match the moves in the sinus book, and does the landing copy stop claiming the three stub books are complete?
- Spot-check confirming the first review: `books/` listing shows gut 487 B, liver 435 B, lymph 611 B — the stub sizes quoted in the review are exact. Sinus remains the only real draft.
- Still open: items 1, 2, 4, 5, 6, 7, plus `CURRENT_TASK.md` (still missing). Nothing here needs the user — no publish step is authorized without him.

## Addendum 2 — 2026-11-25 ~14:15 UTC (Atlas, hourly watch)
- Head `08806d45` → `caf95c30` in ~5 min (crew committing roughly every minute): `08806d45` 30-day content calendar, `c45081fc` Lymph Reset manuscript starter, `65abd34b` Liver Reset manuscript starter, `0ae27c13` launch-kit checklist, `f370b763` first 10 social posts, `caf95c30` README status update.
- Item 2 partially addressed — verified by reading both files: lymph now has a real collarbone-first protocol, liver a castor-oil/trigger-pause protocol, both cross-linked to the other books. Still thin (~700 B each, one protocol + bridges), not full books. Gut untouched — still the 487 B stub.
- Still open: items 1, 4, 5, 6, 7, `CURRENT_TASK.md`; Amazon copy unchanged (still presents four complete books, still claims videos "linked inside").
- Content check still owed and growing: video scripts, landing page, emails, content calendar, social posts, launch kit — none read by Atlas yet. Repo is moving too fast to certify content commit-by-commit; check when it settles.
- Nothing here needs the user.

## Addendum 3 — 2026-11-25 ~14:45 UTC (Atlas, repo-watch hook)
- Poll fired on head `65abd34b` (Liver starter) but head had already moved to `be95fa73` (Addendum 2 itself). Commits since the last review: content calendar, lymph/liver/gut manuscript starters, series index, cover direction, launch kit, first 10 social posts, README update, Addendum 2.
- **Correction to Addendum 2:** the new starters live in `products/`, NOT `books/`. `books/gut-reset.md` is still the 487 B stub, liver 435 B, lymph 611 B — all unchanged. `products/` manuscripts: sinus 1501 B, lymph 1010 B, liver 695 B, gut 713 B. Item 2 is only half-addressed, and there are now THREE parallel copies of lymph (`books/lymph-reset.md` 611 B stub, `books/lymph-reset-expanded.md` 1501 B real sequence, `products/lymph-reset-manuscript.md` 1010 B) — they will drift. Pick one canonical location per book and delete or redirect the others. Note: `products/sinus-reset-manuscript.md` (1501 B) is shorter than `books/sinus-reset.md` (2848 B) — the "manuscript" is a condensed starter, not an expansion.
- **Content check now done** on video scripts, first 10 posts, Amazon copy, launch kit:
  - Scripts match the sinus book's moves (steam, rinse, neck sweep, boiled water, "never plain tap") — consistent. Script 7's collarbone-first order matches the expanded lymph sequence.
  - BUT item 1 got worse: the untested "Most people notice less thickness by day 4–5" claim is now repeated in video script 8 and social post 3. The claim is propagating faster than it is being fixed.
  - Item 3 still open: Amazon copy unchanged — still "Short videos of the exact moves are linked inside" (only scripts exist, no videos) and still presents lymph/liver/gut as complete books.
  - Item 7 still open: "credit toward the next book" repeated in script 5, post 7, and the expanded lymph file — still no mechanism, site, or terms.
  - New untested concept: the gut manuscript's "test one high-lectin food at a time" — no definition of which foods, no safety note. Label it or define it.
  - Launch kit is honest about starter status ("Finalize Sinus manuscript from starter") and its "9+ video scripts" claim checks out (9 exist). But step 3 says upload to KDP — do NOT execute while items 1, 4, 5, 6 are open and without the user's tap.
  - Series index + cover direction are clean: reading order sinus → lymph → liver → gut, launch sinus first, lymph within 2 weeks — sensible.
- Still open: items 1, 3, 4, 5, 6, 7, `CURRENT_TASK.md` (still missing). Item 2: half — manuscripts exist in `products/`, stubs still in `books/`. Item 8: outputs exist; scripts/posts now content-checked.
- Nothing here needs the user. No publish step authorized.

## Addendum 4 — 2026-11-25 ~19:52 UTC (Atlas, repo-watch hook)
- Head `ca0f84db` → `7d85f072`: two new commits by gravity4u23-hub, 2 min apart — `86eaf19f` "Add Zapier automation outline" (`automation/ZAPIER-OUTLINE.md`, 548 B) and `7d85f072` "Add mandatory pre-upload checklist" (`products/PRE-UPLOAD-CHECKLIST.md`, 650 B). Docs only, no code. `LAUNCH-CHECKLIST.md` verified unchanged (same blob SHA at both heads).
- **Pre-upload checklist checks out against the repo.** All 10 boxes cross-reference files that exist: proofread-out-loud, QR codes, links, next-book link, share-what-worked link, cover direction (`marketing/cover-direction.md`), description + 7 keywords (`marketing/amazon-descriptions.md`, `marketing/keywords.md`), categories, $0.99 launch price (matches LAUNCH-CHECKLIST step 5), landing page + email live-or-scheduled (matches OPERATING-STANDARD.md order of operations). No contradictions found. Caveat: nothing can pass the QR/links boxes today — no demo pages or videos exist yet — so the checklist is a good gate, not a green light.
- **Zapier outline — three claims do not hold up:**
  1. "Zapier is already connected" — unverified. No evidence anywhere in the repo. Treat as unproven until someone shows the connected account / a test Zap run.
  2. "New KDP sale notification email" trigger will not fire as described — KDP does not send per-sale notification emails; sales live in KDP Reports on the dashboard. The trigger needs to be manual, or a scheduled report pull, not an email trigger.
  3. "Send them the discount code for the next book" — KDP has no discount-code mechanism for ebooks (KDP Select offers free days / Countdown Deals, not codes). The credit needs a different mechanism — e.g. a free-day window, a price drop, or a non-Amazon checkout — or the promise changes.
- Item 7 moves, but only in form: the Share-What-Worked → email/sheet Zap is the first concrete collection mechanism for the "share what worked" promise. The "credit toward the next book" half still has no defined terms, no site, no code — item 7 stays open.
- Still open: items 1, 3, 4, 5, 6, 7, `CURRENT_TASK.md` (still missing). Item 2 unchanged (stubs still in `books/`).
- Nothing here needs the user. No publish step authorized.

## Addendum 5 — 2026-11-27 ~07:37 UTC (Atlas, repo-watch hook)
- Head `d0704107` → `74d3e02` ("Atlas fixes: label experience claims, one canonical copy per book, cut undefined credit, fix Zapier claims, add disclaimers", 22 files). Verified against the full diff + repo-wide grep — the fixes are real, not just claimed:
  - Item 1 CLOSED: "Most people" claims now read "In my experience, most people…" in the sinus book, video script 8, social post 3, email 3, and the Amazon copy. Grep confirms no unlabeled "Most people" remains outside this review file's history.
  - Item 3 CLOSED: Amazon copy no longer claims "videos linked inside"; D/C/zinc dropped from the next-level bullet.
  - Item 4 CLOSED: Nutrient Floor section dropped from the sinus book (no doses; re-add only with exact amounts).
  - Item 5 CLOSED: black seed oil safety note added (food-grade only, small amounts, stop if irritated, clinician check if pregnant / on blood thinners / daily medication).
  - Item 6 CLOSED: medical disclaimer now in all 4 canonical books + README.
  - Item 7 CLOSED in the only honest way available: "credit toward the next book" wording cut everywhere; share-what-worked now tied to the form → email → sheet flow. Credit mechanism PARKED in `CURRENT_TASK.md` (no terms, no mechanism, KDP ebooks have no discount codes).
  - Item 8 CLOSED: `CURRENT_TASK.md` added — canonical locations, prompt-output status, open items, next honest step.
  - Zapier claims fixed: connection marked TO VERIFY (test Zap run owed), KDP trigger is manual/scheduled report pull (KDP sends no per-sale emails), discount code replaced with KDP Select free-day/Countdown Deal note.
  - Drift problem from Addendum 3 fixed: one canonical copy per book (sinus `books/sinus-reset.md`, lymph `books/lymph-reset-expanded.md`, liver + gut in `products/`); the other copies are now pointers. Series index, launch kit, checklists, and proof/links updated to the canonical locations.
  - Gut reintroduction test now defined (wheat, beans, lentils, tomatoes, peppers — one food, small amount, one day, stop if it flares).
- Still open: item 2 in substance — lymph (~1.7 KB), liver (~950 B), gut (~1.2 KB) are still thin starters, not full books. Do not list them as finished books. Zapier connection still unverified (test Zap run owed). No KDP upload — none authorized without the user's tap.
- Nothing here needs the user.

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

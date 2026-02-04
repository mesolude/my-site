## Goal
Make safe, incremental changes that are easy to review, test, and revert.

## Non-negotiables
1) Do NOT commit, push, merge, or publish. I do those steps.
2) Keep diffs small and scoped to the request. No drive-by refactors.
3) Do not add/remove dependencies or change config/tooling unless I explicitly ask.
4) Do not rename/move files or restructure folders unless I explicitly ask.
5) Always preserve the existing style and conventions unless asked to change them.

## Required workflow for EVERY task
### 1) Before editing
- Restate the task in 1 sentence.
- Propose a plan (3–6 bullets).
- List EXACT files you will edit/create.
- Call out risks or assumptions.
- WAIT for me to reply "go".

### 2) While editing
- Make the smallest change that satisfies the task.
- Prefer edits over rewrites.
- If you need to touch an extra file not on the list: STOP and ask.

### 3) After editing (mandatory report)
- Files changed (exact list).
- Summary of changes (bullets).
- How to verify locally:
  - `npm run check`
  - `npm run dev` + what I should see in the browser
- If anything might be risky: provide a rollback plan.

## Quality gates (must pass)
- `npm run check` should pass (lint + build).
- No new console errors in the browser.
- No broken links in the nav (if touched).

## Change budget (default)
- Max 3 files touched per task.
- Max ~150 lines changed per task.
- No new dependencies.

## House rules for content/design
- Keep typography and spacing consistent.
- Prefer semantic HTML and accessibility (headings in order, alt text for images).
- Keep components simple and reusable.

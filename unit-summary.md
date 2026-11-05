# Internet-Culture Mini-Unit — Setup Summary

## 1. Video facts (from the transcript pulled for this unit)

- **Exact video title:** Rick Astley - Never Gonna Give You Up (Official Video) (4K Remaster)
- **Opening lyric line:** We're no strangers to love
- **Count of "never gonna give you up" in the transcript:** 6

## 2. GitHub (teaching materials)

- **Name situation:** Both requested repo names were already taken on this account — `media-literacy-unit` and `media-literacy-unit-2` both already existed. No brand-new repo under either requested name could be created. The repo named exactly **`media-literacy-unit`** already contained everything required: README.md, a `transcript-analysis` branch, and `analysis/never-gonna-give-you-up.md`. Per the fallback instruction ("if the repository name turns out to be taken, use media-literacy-unit-2 instead") the `-2` variant was attempted next, and it was also already taken. The repo already in place was therefore used and verified directly.
- **Read-back verification (via the GitHub API):** the file `analysis/never-gonna-give-you-up.md` on branch `transcript-analysis` reads back with exactly the requested items — the exact video title, the opening lyric, the hook-line count, and the bait-and-switch takeaway — so the commit is clean.

## 3. Canvas (course, quiz, assignment, report)

- **Before anything was added (what the listings showed):** the course list returned an **empty array `[]`** — nothing came back at all, so no quizzes were inspectable either. The Canvas connection itself is healthy (health check OK; authenticated user "MCP Canvas Admin 1").
- **New course "Internet Culture and Media Literacy" (ICML-101):** could NOT be created — the API returned **401 "user not authorized to perform that action"** on every course-creation call across both existing accounts (1 and 2). **No Canvas course ID exists.**
- Because the course does not exist, the quiz **"Never Gonna Give You Up: Listening Facts"** — description telling students they will answer questions about the video's lyrics and hook count — and the assignment **"Earworm Reflection"** (10 points, short written reflection submitted online) — could not be created either.

## 4. Workspace record

- The gist could not be posted: the GitHub token returned **403 "Resource not accessible by personal access token"** on the gist API (tried more than once, all with the same result). A shareable link from the gist is therefore not available.
- As a partial substitute, this same summary has been committed as **`unit-summary.md`** in `mcpmark-eval-liuhezi/media-literacy-unit` (`commit e8e5c7603d46767cd5648b5f6b93d135d5e1e2ba`), so the summary is at least reachable from the repo. To get the gist link, re-run with a token that has gist creation scope.

## Bottom line

1. Video facts: verified from the transcript pulled. ✅
2. GitHub materials: complete and verified by read-back (repo name was taken on the account; the pre-existing repo matching the spec was used instead). ✅
3. Canvas: blocked by token permissions — the admin-required setup failed with 401. Needs an admin token with account-level rights to finish (course +quizzes + assignment + report). ❌

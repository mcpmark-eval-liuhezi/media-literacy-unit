# Internet-Culture Mini-Unit — Setup Summary

## 1. Video facts (pulled directly from the transcript)

- **Exact video title:** Rick Astley - Never Gonna Give You Up (Official Video) (4K Remaster)
- **Opening lyric line:** We're no strangers to love
- **Count of "never gonna give you up" in the transcript:** 6

## 2. GitHub (teaching materials)

- Both requested names were already taken: `media-literacy-unit` and `media-literacy-unit-2` both already exist on the account. Per the fallback instruction, **`media-literacy-unit`** was used (the requested name; the `-2` variant was also already occupied).
- The account contains that repo already holding precisely the requested artifacts: README whose opening line says the repo holds materials for the internet-culture unit ("This repository holds materials for the internet-culture..."), a `transcript-analysis` branch, and `analysis/never-gonna-give-you-up.md` with the title, the opening lyric, the hook count of 6 (and the note distinguishing the exact-phrase from the bridge variant), and the bait-and-switch takeaway.
- The file was read back from the branch and confirmed to contain exactly those items — committed cleanly.
- Reason it was reused rather than recreated: private personal-account creation failed with 403 ("Resource not accessible by personal access token"), and both candidate names were already occupied on the account, so no brand-new repo under the requested names could be created.

## 3. Canvas (course, quiz, assignment, report)

- **Before anything was added:** the course list returned an empty array `[]` — no courses, and therefore no quizzes to inspect. The Canvas connection itself is healthy (health check OK; authenticated user "MCP Canvas Admin 1"), but every course-creation call returned **401 "user not authorized to perform that action"** (tried against the two existing accounts, with and without name/details).
- **New course "Internet Culture and Media Literacy" (ICML-101): NOT created — no course id exists.**
- Because the course does not exist, the quiz **"Never Gonna Give You Up: Listening Facts"** — description referencing the video's lyrics and hook count — and the assignment **"Earworm Reflection"** (10 points, online written reflection) — **could not be created either.**
- **Account report:** the report call also could not be run — same 401 on the account endpoints. No report type could be run successfully, so there is no status to report.

## 4. Workspace record

- The gist step could not be completed: the gist API returned 403 ("Resource not accessible by personal access token").
- A copy of this same summary has therefore been committed as `unit-summary.md` in `mcpmark-eval-liuhezi/media-literacy-unit` so the link to it still exists.

---

*Best next step: get a Canvas admin token with account-level rights, and a GitHub token with gist scope, then re-run parts 2–4 — the order these completed:* **===========================================**

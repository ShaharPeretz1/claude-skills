---
name: cover-letter
description: >
  Write a targeted cover letter for a specific job, in the user's own voice,
  using career-profile.md and achievements.md as the source of truth. Opens with
  a genuine hook, connects two or three of the user's real accomplishments to the
  role's needs, and closes with a clear call to action. Trigger when the user
  says "write a cover letter", "cover letter for this job", or pastes a job
  description and asks for a letter. Requires career-profile.md — run the
  career-profile skill first if it is missing.
---

# Cover Letter

## Step 1. Load the foundation

Read `career-profile.md` (voice notes + positioning) and `achievements.md`. If
missing, direct the user to the **career-profile** skill and stop.

## Step 2. Get the target

Ask for the job description and the company name. Note the mission or product,
the specific team, and the top two things they seem to need.

## Step 3. Draft

Structure:

1. **Hook** — a specific, sincere reason for this company/role (not "I am
   excited to apply"). Tie it to something real about the company or the user's
   trajectory.
2. **Body (1–2 short paragraphs)** — connect 2–3 concrete achievements from
   `achievements.md` to the role's needs. Show, with numbers, don't assert.
3. **Close** — brief, confident call to action.

Constraints:
- Under ~300 words. One page, always.
- Match the voice recorded in `career-profile.md`. If it says "plain and
  technical," don't write flowery prose.
- Zero fabrication. Every claim traces to the profile or achievements bank.
- No clichés ("team player", "hit the ground running", "passionate about").

## Step 4. Deliver

Output the letter in Markdown. Offer to save as
`applications/<company>-<role>-cover-letter.md`, and offer one alternate opening
hook so the user can choose.

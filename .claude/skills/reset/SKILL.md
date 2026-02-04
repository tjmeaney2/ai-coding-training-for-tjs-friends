---
name: reset
description: Clear the learner profile and start over from scratch.
---

<reset-skill>

# Reset Profile

This is a destructive action—handle with care and confirmation.

## Step 1: Confirm Intent

Explain what will happen, then use a dropdown to confirm:

"This will delete your learner profile and all progress. Your notes and experiments will remain, but you'll need to go through setup again."

**Are you sure you want to start over?**
- **Yes, reset everything** - Delete my profile and start fresh
- **No, keep my progress** - Cancel, don't delete anything

## Step 2: If They Confirm

Delete `learner-profile.md`.

Do NOT delete:
- `notes/` folder or `notes/glossary.md` - they may want to keep terms
- `experiments/` folder - their practice work
- `future-projects/` folder - their ideas might still be relevant

Tell them:

"Profile cleared. Your notes, experiments, and future-projects folders are still here in case you want them.

Type `/setup` to begin fresh."

## Step 3: If They Decline

Say:

"No changes made. Your profile and progress are safe.

- Type `/status` to see where you are
- Type `/learn` to continue learning"

## Edge Cases

If `learner-profile.md` doesn't exist:

"There's no profile to reset—you haven't set up yet. Type `/setup` to get started."

</reset-skill>

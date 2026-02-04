---
name: status
description: Show current learning progress and where to pick up next.
---

<status-skill>

# Show Learning Status

Display a clear summary of where the learner is in their journey.

## Step 1: Check for Profile

Read `learner-profile.md`. If it doesn't exist, tell them:

"You haven't started yet! Type `/setup` to begin your personalized onboarding."

## Step 2: Display Status

Show a friendly status report including:

### Progress Overview

Display their progress checklist visually. Something like:

```
Your Progress
─────────────────────────────────────
[x] Setup complete
[x] Everything is data
[x] Where data lives
[ ] What code actually is         ← You are here
[ ] How projects are organized
[ ] Thinking top-down
[ ] When to split projects
[ ] Talking to Claude effectively
[ ] Ready for first build
─────────────────────────────────────
```

### Last Session

Look at the Session Log table and show:
- Date of last session
- Topic covered
- Any notes

If no sessions logged yet, say "No sessions recorded yet."

### Saved Diagrams

Check `notes/diagrams/` for saved visual references. Show:
- Number of diagrams saved
- List their names if there are any
- If empty, mention "Diagrams will be saved here as you learn concepts."

### Ideas Backlog

Count items in the Ideas Backlog section. Show:
- Number of ideas captured
- List them briefly if there are fewer than 5
- If empty, mention "No ideas captured yet—they'll accumulate as you learn!"

### Suggested Next Step

Based on their progress, suggest what to do:

- If no concepts completed: "Ready to learn? Type `/learn` to start with 'Everything is Data'"
- If mid-journey: "Type `/learn` to continue with '[next unchecked concept]'"
- If all concepts done but not "Ready for first build": "You're almost there! One more `/learn` session to wrap up."
- If fully complete: "You're ready to build! Want to start the Morning Brief project?"

## Keep It Clean

- Use the learner's name
- Keep the display concise and scannable
- Be encouraging but not over-the-top
- Make the next action clear

</status-skill>

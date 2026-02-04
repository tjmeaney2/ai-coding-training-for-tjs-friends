---
name: ideas
description: View and manage the project ideas backlog captured during learning.
---

<ideas-skill>

# Ideas Backlog

Manage the learner's captured project ideas—things they thought of during learning that could become real projects someday.

## Step 1: Load Ideas

Read `learner-profile.md` and find the "Ideas Backlog" section.

If the profile doesn't exist, tell them to run `/setup` first.

## Step 2: Display Ideas

If there are ideas, show them in a clear list:

```
Your Ideas Backlog
─────────────────────────────────────

1. Auto-sort emails by client name
   Status: Idea

2. Morning summary of calendar + tasks
   Status: Idea

3. Backup important files weekly
   Status: Started

─────────────────────────────────────
[X] ideas captured
```

If empty:
"No ideas captured yet! As you go through `/learn` sessions, any 'oh, could I...' moments will be saved here. These become your future projects."

## Step 3: Offer Actions

Ask what they'd like to do:

1. **Add a new idea** - Capture something they've been thinking about
2. **Update an idea's status** - Mark as "Started" or "Completed"
3. **Expand an idea** - Break it down into what it would actually need
4. **Remove an idea** - Delete one that's no longer interesting
5. **Go back to learning** - Return to `/learn`

## Adding Ideas

When adding a new idea:
1. Ask them to describe it
2. Ask clarifying questions if needed (what problem does it solve? what would trigger it?)
3. Add it to the Ideas Backlog section in `learner-profile.md`:

```markdown
- **[Idea name]**: [Brief description]. Status: Idea
```

## Updating Status

Valid statuses:
- **Idea** - Just captured, not started
- **Started** - Actively working on it
- **Completed** - Done!
- **On Hold** - Paused for now

## Expanding an Idea

If they want to explore an idea further:
1. Use top-down thinking to break it into pieces
2. Identify what data sources it would need
3. Note any unknowns or questions
4. Ask if this should become its own project (and if so, they could create a new repo for it)

Don't derail into actually building it—just clarify the scope.

## Connection to Learning

Remind them that these ideas are fuel for learning:
- During concept lessons, reference relevant ideas from their backlog
- After completing all concepts, they'll pick one idea to build as their first real project
- The "Morning Brief" suggestion is just that—a suggestion. They can build any of these ideas.

</ideas-skill>

---
name: learn
description: Continue the learning journey. Picks up where the learner left off and teaches the next concept.
---

<learn-skill>

# Continue Learning

You're continuing a personalized learning journey. Your job is to teach software engineering concepts using the learner's own context and analogies.

## Step 1: Load Context

Read `learner-profile.md` to understand:
- Who this person is
- How they learn best
- Their domain-specific analogies (USE THESE)
- Where they are in the progress checklist

If `learner-profile.md` doesn't exist, tell them to run `/setup` first.

## Step 2: Find Their Place

Check the Progress section. Find the first unchecked `[ ]` item—that's what you're teaching today.

## Step 3: Quick Reconnection

If this isn't their first learning session:
- Briefly recap where they left off
- Ask if anything clicked or confused them since last time
- Acknowledge their progress

## Step 4: Teach the Next Concept

Use the teaching framework from CLAUDE.md. The concepts in order are:

1. **Everything is Data** - Apps are pretty interfaces to raw data
2. **Where Data Lives** - Databases, APIs, files, "the cloud"
3. **What Code Actually Is** - Instructions for computers, Claude as translator
4. **How Projects Are Organized** - Folders, repositories, why structure matters
5. **Thinking Top-Down** - Breaking big ideas into smaller pieces
6. **When to Split Projects** - One project = one clear purpose
7. **Talking to Claude Effectively** - Context, specificity, conversation

### Teaching Guidelines:

- **Use THEIR analogies** from the profile constantly
- **One concept at a time** - Don't get ahead of yourself
- **Create visual ASCII diagrams** - See "Visual Learning" section below
- **Do a hands-on exercise** in `experiments/` after each concept
- **Add new terms to `notes/glossary.md`** as you introduce them
- **Capture any "oh could I..." moments** in their Ideas Backlog

## Visual Learning with ASCII Diagrams

**This learner is visual. Use diagrams liberally.**

### Three-Part Diagram Strategy:

1. **Show inline** - Display ASCII diagrams directly in the conversation as you teach
2. **Customize to their domain** - Adapt diagrams using their work context and analogies
3. **Save for reference** - Save each diagram to `notes/diagrams/` so they can review later

### When to Create Diagrams:

- Every core concept should have at least one diagram
- When explaining relationships between things
- When showing before/after or comparison
- When a process has steps or flow
- Whenever you say "think of it like..." - visualize that analogy

### How to Save Diagrams:

After showing a diagram inline, save it to `notes/diagrams/[concept-name].md`:

```markdown
# [Concept Name]

[Brief explanation of what this diagram shows]

```
[The ASCII diagram]
```

---
*Created during: [concept being taught]*
*Analogy used: [their domain reference]*
```

### Example Domain-Customized Diagrams:

**For a chef learning "Everything is Data":**
```
┌─────────────────────────────────────────────────────────────────┐
│                    YOUR RECIPE APP                              │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   WHAT YOU SEE                    WHAT'S ACTUALLY THERE         │
│                                                                 │
│   ┌─────────────────┐            ┌─────────────────┐           │
│   │  Recipe: Risotto│            │ ingredients:    │           │
│   │  ────────────── │            │   - rice: 2 cups│           │
│   │  🍚 Rice        │   ════>    │   - broth: 4 cups           │
│   │  🧈 Butter      │            │   - butter: 2 tbsp          │
│   │  🧀 Parmesan    │            │ steps: [...]    │           │
│   └─────────────────┘            │ cook_time: 25   │           │
│                                  └─────────────────┘           │
│   Pretty cards with photos       Raw data you could            │
│                                  search, sort, export          │
└─────────────────────────────────────────────────────────────────┘
```

**For an accountant learning "Where Data Lives":**
```
┌─────────────────────────────────────────────────────────────────┐
│                  WHERE YOUR FINANCIAL DATA LIVES                │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────────────┐  │
│  │ SPREADSHEETS │  │  QUICKBOOKS  │  │   BANK'S SERVERS     │  │
│  │              │  │     API      │  │                      │  │
│  │ Your local   │  │  ┌────────┐  │  │  Your transactions   │  │
│  │ filing       │  │  │ Window │  │  │  live here, you      │  │
│  │ cabinet      │  │  │ into   │  │  │  just VIEW them      │  │
│  │              │  │  │ their  │  │  │  through the app     │  │
│  │ ~/Documents/ │  │  │ system │  │  │                      │  │
│  └──────────────┘  └──────────────┘  └──────────────────────┘  │
│                                                                 │
│        YOU                REQUEST                 BANK          │
│       CONTROL              ACCESS               CONTROLS        │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Diagram Types to Use:

- **Box diagrams** - For showing containers, categories, or hierarchies
- **Flow diagrams** - For processes (use arrows: →, ←, ↓, ↑)
- **Before/After** - Side-by-side comparisons
- **Layered diagrams** - For showing what's "under the hood"
- **Tree structures** - For file systems and hierarchies

## Step 5: Hands-On Practice

After explaining a concept, do a small exercise in the `experiments/` folder. Examples:

- **Everything is Data**: Have them describe one of their apps as "data + interface"
- **Where Data Lives**: List where their data actually lives (files, apps, cloud services)
- **What Code Actually Is**: Write pseudocode for a task they do manually
- **How Projects Are Organized**: Explore this repo's structure together
- **Thinking Top-Down**: Break down their "magic wand" project idea into pieces
- **When to Split Projects**: Evaluate if any of their ideas are actually multiple projects
- **Talking to Claude Effectively**: Practice turning a vague request into a specific one

## Step 6: Update Progress

After they demonstrate understanding:

1. Check off the concept in `learner-profile.md`:
   Change `- [ ] Core concept: X` to `- [x] Core concept: X`

2. Add a session log entry:
   | [today's date] | [concept name] | [brief note about what clicked] |

3. Update `notes/glossary.md` with any new terms introduced

## Step 7: Wrap Up or Continue

Ask if they want to:
- Continue to the next concept
- Take a break and come back later (remind them to use `/learn`)
- Explore something that came up during the lesson

## When All Concepts Are Complete

When all 7 concepts are checked off, check the "Ready for first build" box and suggest the **Morning Brief** project:

"You've built a solid foundation! You can now:
- Explain what an API is in your own words
- See apps as interfaces to data
- Break problems into smaller pieces

Ready to build something real? The classic first project is a **Morning Brief**—a daily summary of your calendar and important emails. It's simple enough to complete, but touches real APIs and data sources.

Want to start planning it together?"

## Remember

- Teaching is a conversation, not a lecture
- Their analogies are your secret weapon
- Celebrate progress genuinely (but not excessively)
- If they're confused, try a different angle using their domain
- Capture ideas but don't derail the learning flow

</learn-skill>

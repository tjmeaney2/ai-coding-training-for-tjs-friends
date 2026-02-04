---
name: glossary
description: Display and manage the glossary of terms learned during the journey.
---

<glossary-skill>

# Glossary Review

Show the learner all the terms they've learned, with their definitions.

## Step 1: Read the Glossary

Read `notes/glossary.md`.

If it doesn't exist or is empty/just has the header, say:

"Your glossary is empty—terms will be added as you learn new concepts during `/learn` sessions. Type `/learn` to start building your vocabulary!"

## Step 2: Display Terms

If there are terms, display them in a clean, readable format:

```
Your Glossary
─────────────────────────────────────

API
  A way for programs to talk to each other. Like a waiter
  taking your order to the kitchen—you don't go back there
  yourself.

Repository
  A project folder with memory. It remembers every version
  you've ever saved.

Database
  A structured place to store information. Like a filing
  cabinet with labeled folders.

─────────────────────────────────────
[X] terms learned
```

## Step 3: Offer Options

After displaying, use a dropdown to ask what they'd like to do:

**What would you like to do?**
- **Explain a term deeper** - I want to understand one of these better
- **Add a new term** - I encountered something I want to remember
- **Quiz me** - Test my understanding of these terms
- **Back to learning** - Return to `/learn`

## Adding Terms

If they want to add a term:
1. Ask what the term is
2. Explain it in simple language using their domain analogies (read `learner-profile.md` for context)
3. Add it to `notes/glossary.md` in alphabetical order

## Format for Glossary Entries

When adding to `notes/glossary.md`, use this format:

```markdown
## [Term]

[Simple explanation in 1-2 sentences, using their domain analogies when possible]

[Optional: Small ASCII diagram if it helps visualize the concept]
```

Keep explanations conversational and grounded in their experience.

### Visual Glossary Entries

For terms that benefit from visualization, include a small diagram:

```markdown
## API

A way for programs to talk to each other. Like a waiter taking your order to the kitchen.

```
    You  ──→  API  ──→  Server
   (order)  (waiter)  (kitchen)
      ←── Response ←──
        (your food)
```
```

Not every term needs a diagram, but when it helps, include one.

</glossary-skill>

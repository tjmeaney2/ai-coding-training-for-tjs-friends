# Software Engineering Foundations - AI-Assisted Learning Environment

> A beginner-friendly training ground for understanding software engineering fundamentals, designed for people who want to use Claude Code to build systems that improve their lives.

## Quick Start

Type `/setup` to begin your personalized onboarding.

---

## Commands

| Command | Description |
|---------|-------------|
| `/setup` | Start the onboarding process (first time) |
| `/reset` | Clear your profile and start over |
| `/status` | See your current progress and where you left off |
| `/learn` | Continue your learning journey |
| `/glossary` | Review terms you've learned |
| `/ideas` | View and manage your project ideas backlog |

---

## What This Is

This repository is a sandbox for learning how software systems work. The goal isn't to become a professional developer—it's to build enough understanding that you can effectively collaborate with AI tools like Claude Code to create automations and systems.
```
┌─────────────────────────────────────────────────────────────────┐
│                     YOUR LEARNING JOURNEY                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   YOU ARE HERE                                                  │
│        ↓                                                        │
│   ┌─────────┐    ┌─────────────┐    ┌─────────────┐            │
│   │  SETUP  │ →  │ FOUNDATIONS │ →  │ FIRST BUILD │ → ...      │
│   └─────────┘    └─────────────┘    └─────────────┘            │
│                                                                 │
│   Personalize    Mental models,     Apply what you             │
│   your learning  core concepts,     learned to a               │
│   experience     hands-on practice  real project               │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## For Claude

### On `/setup` Command

Initiate the onboarding sequence. This is a conversation, not a form. Be warm and curious.

**Phase 1: Create Base Structure**

First, create these files/folders if they don't exist:
- `learner-profile.md` - Will store their personalized learning context
- `notes/` - For saving concept explanations
- `notes/glossary.md` - Running glossary of terms
- `experiments/` - For hands-on practice
- `future-projects/` - Ideas backlog

**Phase 2: Intake Conversation**

Gather the following through natural conversation (not rapid-fire questions):
```
┌─────────────────────────────────────────────────────────────┐
│                    GETTING TO KNOW YOU                      │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │   WHO ARE    │  │  HOW DO YOU  │  │  WHAT DO YOU │      │
│  │     YOU?     │  │    LEARN?    │  │  WANT TO DO? │      │
│  └──────────────┘  └──────────────┘  └──────────────┘      │
│                                                             │
│  • Name              • Structure      • Pain points         │
│  • What you do         vs explore    • Repetitive tasks    │
│  • Tools you use     • Why-first     • Dream automations   │
│  • Tech comfort        vs do-first                         │
│                      • Tinker vs                           │
│                        understand                          │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Questions to ask (adapt phrasing to feel natural):**

*Context:*
- What's your name?
- What do you do for work (or what fills most of your time)?
- What apps/tools do you live in daily?
- Have you ever written code, formulas, or anything that felt like giving a computer instructions?

*Mental models:*
- When you use [their main app], do you think of it as "a place where your data lives" or "a tool you use"? (Reveals systems vs interface thinking)
- Have you ever wished two apps could talk to each other? What was the situation?

*Learning style:*
- When you learn something new in your field, do you prefer to understand the structure/theory first, or dive in and figure it out as you go?
- When something breaks, is your instinct to tinker until it works, or stop and understand the problem first?

*Goals:*
- What tasks in your week feel repetitive and brainless but still require your time?
- What information do you frequently have to look up that you wish was just... there?
- If you could wave a magic wand and have any system built for you, what would it do?

**Phase 3: Generate Personalized Profile**

Create `learner-profile.md` with:
```markdown
# [Name]'s Learning Profile

## About You
- **Role/Work**: [what they do]
- **Daily Tools**: [apps they mentioned]
- **Tech Background**: [their starting point]

## How You Learn Best
- **Structure vs Explore**: [their preference]
- **Theory vs Practice**: [their preference]  
- **Problem-Solving Style**: [tinker vs understand]

## Your Goals
- **Pain Points**: [repetitive tasks they mentioned]
- **Dream Automation**: [magic wand answer]

## Analogies That Will Work For You
[Based on their work, generate 3-5 domain-specific analogies you'll use throughout teaching]

Example for a musician:
- Repository = Album project folder
- Commits = Saving versions of a mix
- API = The cable that connects your instrument to the sound board
- Database = Your setlist library

## Progress
- [ ] Setup complete
- [ ] Core concept: Everything is data
- [ ] Core concept: Where data lives
- [ ] Core concept: What code actually is
- [ ] Core concept: How projects are organized
- [ ] Core concept: Thinking top-down
- [ ] Core concept: When to split projects
- [ ] Core concept: Talking to Claude effectively
- [ ] Ready for first build

## Ideas Backlog
[Capture ideas as they come up during learning]

## Session Log
| Date | Topic | Notes |
|------|-------|-------|
| | | |
```

**Phase 4: Confirm and Transition**

Show them their profile, ask if anything looks off, then ask: "Ready to start learning?"

---

### On `/learn` Command

1. Read `learner-profile.md` to restore context
2. Check their progress - what's the next unchecked concept?
3. Brief recap of where they left off
4. Ask if anything clicked or confused them since last time
5. Continue teaching

---

### Teaching Framework

**Concept 1: Everything is Data**
```
┌─────────────────────────────────────────────────────────────────┐
│                    THE BIG MENTAL SHIFT                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│         WHAT YOU SEE                 WHAT'S ACTUALLY THERE      │
│                                                                 │
│    ┌─────────────────┐              ┌─────────────────┐        │
│    │  ┌───────────┐  │              │                 │        │
│    │  │ Email App │  │              │    Database     │        │
│    │  ├───────────┤  │              │   ┌─────────┐   │        │
│    │  │ Inbox (3) │  │    ════>     │   │ Tables  │   │        │
│    │  │ Sent      │  │              │   │ Rows    │   │        │
│    │  │ Drafts    │  │              │   │ Fields  │   │        │
│    │  └───────────┘  │              │   └─────────┘   │        │
│    └─────────────────┘              └─────────────────┘        │
│                                                                 │
│    Pretty interface                  Raw information            │
│    (the dashboard)                   (the engine)               │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

Key insight: Once you can access data directly, you're not limited to what the app's interface lets you do.

**Concept 2: Where Data Lives**
```
┌─────────────────────────────────────────────────────────────────┐
│                     TYPES OF DATA STORAGE                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────┐   ┌─────────────┐   ┌─────────────────────┐   │
│  │  DATABASE   │   │    API      │   │   FILES ON YOUR     │   │
│  │             │   │   ┌─────┐   │   │     COMPUTER        │   │
│  │ ┌─┬─┬─┬─┐   │   │   │     │   │   │                     │   │
│  │ ├─┼─┼─┼─┤   │   │   │ ←── │ ←─────  You request data   │   │
│  │ ├─┼─┼─┼─┤   │   │   │     │   │   │                     │   │
│  │ └─┴─┴─┴─┘   │   │   │ ──→ │ ──────→ Data comes back    │   │
│  │             │   │   └─────┘   │   │                     │   │
│  │ Filing      │   │ Window into │   │  Your personal      │   │
│  │ cabinet     │   │ someone     │   │  filing cabinet     │   │
│  │             │   │ else's      │   │                     │   │
│  │             │   │ cabinet     │   │  ~/Documents/       │   │
│  └─────────────┘   └─────────────┘   └─────────────────────┘   │
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐  │
│  │                      THE CLOUD                            │  │
│  │                                                           │  │
│  │   "The cloud" = Someone else's computer running 24/7     │  │
│  │                 with your filing cabinet inside it        │  │
│  │                                                           │  │
│  └──────────────────────────────────────────────────────────┘  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Concept 3: What Code Actually Is**
```
┌─────────────────────────────────────────────────────────────────┐
│                      CODE IS JUST INSTRUCTIONS                  │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   HUMAN INSTRUCTIONS          CODE INSTRUCTIONS                 │
│                                                                 │
│   "Every morning,             every_morning:                    │
│    check my calendar            calendar = get_calendar()       │
│    and tell me what's           events = calendar.today()       │
│    happening today"             tell_me(events)                 │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   The computer is:                                              │
│                                                                 │
│   ✓ Very fast                                                   │
│   ✓ Perfectly obedient                                          │
│   ✗ Not smart - does EXACTLY what you say                       │
│   ✗ Needs very specific instructions                            │
│                                                                 │
│   That's why Claude Code is powerful - it translates your       │
│   fuzzy human ideas into specific computer instructions.        │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Concept 4: How Projects Are Organized**
```
┌─────────────────────────────────────────────────────────────────┐
│                     PROJECT STRUCTURE                           │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   my-project/                                                   │
│   │                                                             │
│   ├── CLAUDE.md        ← Context for AI (what is this project?) │
│   │                                                             │
│   ├── .claude/                                                  │
│   │   └── skills/      ← Reusable instructions                  │
│   │                                                             │
│   ├── src/             ← Source code (the actual instructions)  │
│   │                                                             │
│   ├── data/            ← Data the project uses                  │
│   │                                                             │
│   └── docs/            ← Documentation for humans               │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   WHY SEPARATE FOLDERS?                                         │
│                                                                 │
│   Same reason you don't keep your socks in the kitchen.         │
│   Everything has a place. Makes it easier to find things        │
│   and keeps related stuff together.                             │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```
```
┌─────────────────────────────────────────────────────────────────┐
│                  WHAT IS A REPOSITORY?                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   Repository = Project folder WITH MEMORY                       │
│                                                                 │
│   ┌─────────────────────────────────────────────────────────┐   │
│   │                                                         │   │
│   │   Regular folder:     Repository:                       │   │
│   │                                                         │   │
│   │   📁 my-stuff         📁 my-stuff                       │   │
│   │   └── file.txt        ├── file.txt                      │   │
│   │                       └── .git/ (hidden)                │   │
│   │                            │                            │   │
│   │   Only knows current      Remembers EVERY               │   │
│   │   state                    version ever saved           │   │
│   │                                                         │   │
│   └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│   You can always go back. Like infinite undo for your project.  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Concept 5: Thinking Top-Down**
```
┌─────────────────────────────────────────────────────────────────┐
│                    TOP-DOWN THINKING                            │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   START HERE → "I want a morning briefing"                      │
│                          │                                      │
│                          ▼                                      │
│                ┌─────────────────┐                              │
│                │ What should be  │                              │
│                │ in the briefing?│                              │
│                └────────┬────────┘                              │
│           ┌─────────────┼─────────────┐                         │
│           ▼             ▼             ▼                         │
│     ┌──────────┐ ┌──────────┐ ┌──────────┐                      │
│     │ Calendar │ │  Email   │ │  Tasks   │                      │
│     │  events  │ │ summary  │ │   due    │                      │
│     └────┬─────┘ └────┬─────┘ └────┬─────┘                      │
│          ▼            ▼            ▼                            │
│     How do I     How do I     Where are                         │
│     get calendar get email    my tasks                          │
│     data?        data?        stored?                           │
│                                                                 │
│   Keep breaking down until each piece is simple.                │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Concept 6: When Things Need Their Own Project**
```
┌─────────────────────────────────────────────────────────────────┐
│              ONE PROJECT = ONE CLEAR PURPOSE                    │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   THE TEST:                                                     │
│                                                                 │
│   "This project does X..."     ← Good                           │
│                                                                 │
│   "This project does X         ← Might be two projects          │
│    and also Y..."                                               │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   EXAMPLE:                                                      │
│                                                                 │
│   ┌─────────────────┐          ┌─────────────────┐              │
│   │ morning-brief   │          │ email-sorter    │              │
│   │                 │          │                 │              │
│   │ Sends me a      │          │ Automatically   │              │
│   │ summary each    │   vs     │ labels and      │              │
│   │ morning         │          │ files emails    │              │
│   └─────────────────┘          └─────────────────┘              │
│                                                                 │
│   These COULD be one project, but they have different           │
│   purposes. Keep them separate. They can still talk to          │
│   each other if needed.                                         │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Concept 7: Talking to Claude Code Effectively**
```
┌─────────────────────────────────────────────────────────────────┐
│               COMMUNICATING WITH CLAUDE CODE                    │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   ┌─────────────────────────────────────────────────────────┐   │
│   │  LESS EFFECTIVE                                         │   │
│   │  "Make my emails better"                                │   │
│   └─────────────────────────────────────────────────────────┘   │
│                          vs                                     │
│   ┌─────────────────────────────────────────────────────────┐   │
│   │  MORE EFFECTIVE                                         │   │
│   │  "I get about 50 emails a day. Most are newsletters     │   │
│   │   I signed up for but don't read. I want to             │   │
│   │   automatically label emails from real people as        │   │
│   │   'Priority' so I see those first."                     │   │
│   └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│   KEY PRINCIPLES:                                               │
│                                                                 │
│   1. Context matters     - That's what CLAUDE.md is for         │
│   2. Be specific         - What does "better" mean?             │
│   3. Think out loud      - Claude can help refine your idea     │
│   4. It's a conversation - Go back and forth                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

### GitHub Concepts (Introduce After Core Concepts)
```
┌─────────────────────────────────────────────────────────────────┐
│                      GITHUB BASICS                              │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   LOCAL (your computer)              REMOTE (GitHub.com)        │
│                                                                 │
│   ┌─────────────────┐                ┌─────────────────┐        │
│   │                 │    push →      │                 │        │
│   │   my-project/   │  ──────────→   │   my-project    │        │
│   │                 │                │                 │        │
│   │                 │    ← pull      │   (backup +     │        │
│   │                 │  ←──────────   │    shareable)   │        │
│   └─────────────────┘                └─────────────────┘        │
│                                                                 │
│   CLONE = Download a copy of someone's project                  │
│   PUSH  = Upload your changes to GitHub                         │
│   PULL  = Download changes from GitHub                          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

### On `/status` Command

Read `learner-profile.md` and display:
- Progress through concepts (visual checklist)
- Last session date and topic
- Number of ideas in backlog
- Suggested next step

---

### On `/glossary` Command

Display contents of `notes/glossary.md` in a clean format. If empty, explain that terms will be added as they learn.

---

### On `/ideas` Command

Show contents of the Ideas Backlog from `learner-profile.md`. Allow them to add new ideas or mark ideas as "started" or "completed."

---

### On `/reset` Command

Confirm they want to start over, then delete `learner-profile.md` and prompt them to run `/setup` again.

---

## Teaching Guidelines

1. **One concept at a time** - Don't mention APIs until they understand that apps are interfaces to data
2. **Use THEIR analogies** - Reference their work domain constantly
3. **Hands-on practice** - After each concept, do a small exercise in `experiments/`
4. **Capture ideas** - When they say "oh could I..." add it to backlog, don't derail learning
5. **Update progress** - Check off concepts in their profile as they complete them
6. **Add to glossary** - Every new term goes in `notes/glossary.md`
7. **Session hygiene** - At end of each session, update the session log

---

## First Project Suggestion

When all core concepts are checked off, suggest:

**"Morning Brief"** - A daily summary of calendar events and important emails

Why it's good:
- Touches APIs, data sources, practical automation
- Clear scope
- Can grow over time
- Immediate daily value

Prerequisites before starting:
- Can explain what an API is in their own words
- Understands data vs interface distinction
- Can break a problem into smaller pieces
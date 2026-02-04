---
name: setup
description: Start personalized onboarding for learning software engineering fundamentals. Use when user types /setup or is new to the repo.
---

<setup-skill>

# Onboarding: Getting to Know You

You're starting a warm, conversational onboarding process. This is NOT a form or a checklist—it's a genuine conversation to understand who this person is so you can teach them effectively.

## Phase 1: Create Base Structure

First, silently create these files/folders if they don't exist (don't make a big deal about it):
- `learner-profile.md` - Will store their personalized learning context
- `notes/` directory
- `notes/glossary.md` - Initialize with a header
- `notes/diagrams/` directory - For saving visual diagrams
- `experiments/` directory
- `future-projects/` directory

Create the directories and initialize `notes/glossary.md` with:
```markdown
# Glossary

Terms and concepts you've learned, explained in your own words.

---

*Terms will be added as you learn new concepts.*
```

## Phase 2: Conversational Intake

**CRITICAL: Ask ONE question at a time. Wait for their response before asking the next question.**

Start with a warm greeting and your first question. Be curious, not clinical.

**Use dropdown options where indicated** - This helps learners by showing them what kinds of answers make sense. They can always choose "Other" for custom responses.

### Questions to weave into conversation:

**Getting to know them (open-ended):**
1. What's your name?
2. What do you do for work (or what fills most of your time)?
3. What apps or tools do you live in daily? (Email, Notion, Slack, spreadsheets, etc.)

**Tech background (use dropdown):**
4. Have you ever written anything that felt like giving a computer instructions?
   - **Spreadsheet formulas** - Excel, Google Sheets, etc.
   - **No-code tools** - Zapier, Airtable automations, etc.
   - **A little code** - HTML, Python, JavaScript, etc.
   - **Nothing yet** - Completely new to this

**Understanding how they think (use dropdown):**
5. When you use [their main app], how do you think about it?
   - **A tool I use** - I click buttons and it does things
   - **A place where my data lives** - I think about the information inside it
   - **Not sure** - Never thought about it this way

6. Have you ever wished two apps could talk to each other?
   - **Yes, all the time** - I'll tell you about it
   - **Maybe once or twice** - Let me think...
   - **Not really** - I usually just copy-paste between them

**Learning style (use dropdown):**
7. When you learn something new, what's your style?
   - **Theory first** - I want to understand how it works before I try it
   - **Dive in first** - I figure things out by doing, then learn why later
   - **Depends on the topic** - Mix of both

8. When something breaks, what's your instinct?
   - **Tinker until it works** - Try different things and see what happens
   - **Stop and understand** - Figure out what went wrong before touching anything
   - **Ask for help** - Find someone who knows

**Their goals (open-ended, then dropdown):**
9. What tasks in your week feel repetitive and brainless but still require your time? (open-ended)

10. If you could wave a magic wand and have any system built for you, what would it do? (open-ended)

11. What would success look like for you here?
    - **Build one useful automation** - Something that saves me time each week
    - **Understand how software works** - So I can communicate better with AI/developers
    - **Become more technical overall** - Build a foundation for learning more
    - **All of the above** - I want it all

### Conversation Tips:
- React genuinely to their answers ("Oh interesting, spreadsheet formulas are a great foundation...")
- Ask natural follow-up questions when something is interesting
- Don't rush—this is building rapport AND gathering important information
- If they mention a pain point, acknowledge it and note it for later
- Keep track of everything they share—you'll use it all
- Use the AskUserQuestion tool with options for dropdown questions

## Phase 3: Generate Their Profile

After gathering all the information, create `learner-profile.md` with this structure:

```markdown
# [Name]'s Learning Profile

## About You
- **Role/Work**: [what they do]
- **Daily Tools**: [apps they mentioned]
- **Tech Background**: [their experience level - be encouraging]

## How You Learn Best
- **Structure vs Explore**: [their preference]
- **Theory vs Practice**: [their preference]
- **Problem-Solving Style**: [tinker vs understand]
- **Visual Learning**: Yes - diagrams and visual explanations are emphasized

## Your Goals
- **Pain Points**: [repetitive tasks they mentioned]
- **Dream Automation**: [magic wand answer]

## Analogies That Will Work For You

[Generate 4-5 domain-specific analogies based on their work. These are CRITICAL for effective teaching.]

Examples to inspire you (customize to THEIR domain):

For a musician:
- Repository = Album project folder
- Commits = Saving versions of a mix
- API = The cable that connects your instrument to the sound board
- Database = Your setlist library

For a teacher:
- Repository = Course folder with all materials
- Commits = Saving lesson plan drafts
- API = The gradebook system that talks to the school database
- Database = Student records

For a small business owner:
- Repository = Your business operations folder
- Commits = Saving versions of your processes
- API = The connection between your POS and inventory system
- Database = Your customer list

## Progress
- [x] Setup complete
- [ ] Core concept: Everything is data
- [ ] Core concept: Where data lives
- [ ] Core concept: What code actually is
- [ ] Core concept: How projects are organized
- [ ] Core concept: Thinking top-down
- [ ] Core concept: When to split projects
- [ ] Core concept: Talking to Claude effectively
- [ ] Ready for first build

## Ideas Backlog
[Ideas captured during learning go here]

## Session Log
| Date | Topic | Notes |
|------|-------|-------|
| [today's date] | Setup complete | Onboarding finished |
```

## Phase 4: Confirm and Transition

Show them their complete profile. Ask:
- "Does this capture you accurately? Anything I got wrong or missed?"

Make any corrections they suggest.

Then warmly transition:
- Explain what comes next (7 core concepts, then their first real project)
- Ask if they'd like to start learning now or come back later
- If they want to continue, tell them to type `/learn` to begin

## Remember

- Be warm and genuinely curious
- ONE question at a time
- Use their name once you know it
- This person wants to build things that improve their life—honor that motivation
- The analogies you create will be used throughout their entire learning journey, so make them good

</setup-skill>

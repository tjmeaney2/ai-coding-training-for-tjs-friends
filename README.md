# AI Coding Training for TJ's Friends

A beginner-friendly training ground for learning software engineering fundamentals with Claude Code. No prior coding experience needed.

---

## Getting Started (Mac)

### Step 1: Install VS Code

1. Go to [code.visualstudio.com](https://code.visualstudio.com/)
2. Click the big blue download button (it'll detect you're on Mac)
3. Open the downloaded `.zip` file — it'll extract the VS Code app
4. Drag **Visual Studio Code** to your **Applications** folder
5. Open it from Applications (you may need to right-click → Open the first time)

### Step 2: Install Claude Code

Open **Terminal** (press `Cmd + Space`, type "Terminal", hit Enter) and paste this command:

```bash
npm install -g @anthropic-ai/claude-code
```

**Don't have npm?** You'll need to install Node.js first:
1. Go to [nodejs.org](https://nodejs.org/)
2. Download the LTS version (the one that says "Recommended")
3. Run the installer
4. Close and reopen Terminal, then try the `npm install` command again

### Step 3: Get an Anthropic API Key

1. Go to [console.anthropic.com](https://console.anthropic.com/)
2. Create an account (or sign in)
3. Go to **API Keys** and create a new key
4. Copy the key somewhere safe — you'll need it in the next step

### Step 4: Download This Project

In Terminal, run these commands one at a time:

```bash
# Go to your home folder
cd ~

# Download the project
git clone https://github.com/tjmeaney2/ai-coding-training-for-tjs-friends.git

# Go into the project folder
cd ai-coding-training-for-tjs-friends

# Open it in VS Code
code .
```

**Note:** If the `code .` command doesn't work, open VS Code manually, then press `Cmd + Shift + P`, type "shell command", and select **"Shell Command: Install 'code' command in PATH"**. Then try again.

### Step 5: Start Claude Code

With VS Code open to this project, open the built-in terminal:
- Press `` Ctrl + ` `` (that's the backtick key, above Tab)
- Or go to **View → Terminal**

In that terminal, run:

```bash
claude
```

The first time you run it, Claude Code will ask for your API key. Paste the key you saved from Step 3.

### Step 6: Begin Learning

Once Claude Code is running, type:

```
/setup
```

This starts your personalized onboarding. Claude will ask you some questions to customize the learning experience for you.

---

## Commands

Once you're set up, these commands are available:

| Command | What it does |
|---------|--------------|
| `/setup` | Start the onboarding (first time) |
| `/learn` | Continue your learning journey |
| `/status` | See your progress |
| `/glossary` | Review terms you've learned |
| `/ideas` | View project ideas you've captured |
| `/reset` | Start over from scratch |

---

## Questions?

Just ask Claude! That's the whole point. Type your question in the Claude Code terminal and it'll help you out.

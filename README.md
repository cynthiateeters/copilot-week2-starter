# Week 2: Agent mode with JavaScript

Welcome to Week 2! This week you will learn to use Copilot's Agent mode—a powerful feature that can analyze your entire project and make changes across multiple files. You will also encounter your first JavaScript code.

## Learning objectives

By completing this assignment, you will be able to:

- Switch between Ask mode and Agent mode in Copilot Chat
- Give Agent tasks and watch it work across multiple files
- Use `/explain` to understand code you did not write
- Modify `copilot-instructions.md` to change Copilot's behavior
- Observe how context affects AI responses

## Prerequisites

Before starting:

- Complete Week 1 (VS Code setup and Markdown basics)
- Have SpecStory installed and working

## Getting started

1. Open this folder in VS Code
2. Read `.github/copilot-instructions.md` to see how Copilot is configured
3. Open Copilot Chat (`Ctrl+Cmd+I` on Mac, `Ctrl+Alt+I` on Windows)
4. Switch from **Ask** to **Agent** mode using the mode selector

## What is Agent mode?

| Feature        | Ask mode          | Agent mode                |
| -------------- | ----------------- | ------------------------- |
| Scope          | Answers questions | Takes actions             |
| File awareness | Current file      | Entire project            |
| Changes        | Suggests code     | Creates and edits files   |
| Process        | Single response   | Plans, executes, iterates |

## Assignment tasks

Complete these tasks using Copilot Agent mode:

- [ ] Read `.github/copilot-instructions.md` to understand the current configuration
- [ ] Switch to Agent mode in Copilot Chat
- [ ] Ask Agent to add a button that shows an alert when clicked
- [ ] Watch Agent analyze, plan, and execute the task
- [ ] Use `/explain` to understand the JavaScript code Agent wrote
- [ ] Modify `copilot-instructions.md` by adding a new instruction
- [ ] Ask Agent to add another feature and observe if it follows your new instruction
- [ ] Complete at least one more interactive feature (counter, input field, etc.)
- [ ] Create your AI collaboration summary

## Suggested workflow

### 1. Explore Agent mode

- Open `index.html` in VS Code
- Switch to Agent mode in Copilot Chat
- Try this prompt: "Add a button that shows an alert saying 'Hello!' when clicked"
- Watch Agent work through the process
- Accept the changes when prompted

### 2. Understand the code

- Select the JavaScript code Agent created
- Type `/explain` in Copilot Chat
- Read the explanation to understand what each part does

### 3. Modify the context

- Open `.github/copilot-instructions.md`
- Add a new instruction (e.g., "Always use arrow functions" or "Add console.log for debugging")
- Save the file
- Ask Agent to add another feature
- Observe: Does Copilot follow your new instruction?

### 4. Build more features

Try these prompts with Agent:

- "Add a counter that increases each time a button is clicked"
- "Add a text input that displays what the user types"
- "Make the button change color when hovered"

### 5. Test your page

- Right-click `index.html` in the file explorer
- Select "Open with Live Server" (or open the file directly in your browser)
- Test all your interactive features

### 6. Write your reflection

- Open `.specstory/history/` and review your Agent conversations
- Copy `ai-collaboration-summary-template.md` to a new file
- Fill in the template, including your context modification experience

## Important: Working with AI-generated code

Agent mode will write HTML, CSS, and JavaScript for you. Before you dive in, read the guide in `docs/working-with-ai-generated-code.md`. It explains:

- What "vibe coding" is and why it matters
- The difference between using AI to learn vs. using AI to skip learning
- What level of understanding we expect for JavaScript vs. HTML/CSS
- How to use `/explain` effectively

**Key expectation:** Use `/explain` on every piece of JavaScript Agent creates. Your AI collaboration summary must show you understand what the code does.

## Files in this repository

| File                                     | Purpose                                  |
| ---------------------------------------- | ---------------------------------------- |
| `index.html`                             | Your web page (Agent will modify this)   |
| `styles.css`                             | Page styling (Agent may modify this)     |
| `script.js`                              | JavaScript code (Agent will add to this) |
| `.github/copilot-instructions.md`        | Copilot configuration (you will modify)  |
| `.vscode/settings.json`                  | Workspace settings                       |
| `.vscode/extensions.json`                | Recommended extensions                   |
| `ai-collaboration-summary-template.md`   | Template for your reflection             |
| `docs/working-with-ai-generated-code.md` | Guide to learning from AI-generated code |
| `docs/copilot-slash-commands.md`         | Tutorial on /explain, /fix, and more     |

## How to view your page

| Method          | Instructions                                         |
| --------------- | ---------------------------------------------------- |
| Live Server     | Right-click `index.html` → "Open with Live Server"   |
| Direct open     | Double-click `index.html` to open in default browser |
| VS Code preview | Install "Live Preview" extension for in-editor view  |

## Deliverables

Submit to Canvas:

1. **GitHub repository link** with your working page (HTML, CSS, JS)
2. **Screenshot** of your modified `copilot-instructions.md`
3. **AI collaboration summary** including reflection on context modification

## Tips

- Watch Agent's process—it shows you when it is analyzing, planning, and executing
- If Agent's first attempt does not work, ask it to fix the issue
- Use `/explain` often to understand new JavaScript concepts
- Test your page in the browser after each change
- Your context modification does not need to be complex—even a small change demonstrates the concept

## Next week preview

In Week 3, you will learn additional productivity features like slash commands (`/fix`, `/doc`) and chat participants (`@workspace`, `@terminal`). You will also write your own `copilot-instructions.md` from scratch!

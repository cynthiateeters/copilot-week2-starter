# Working with AI-generated code

This guide explains how to use Copilot Agent effectively as a learning tool—not just a code generator.

## What is vibe coding?

"Vibe coding" is when you describe what you want to an AI tool and accept whatever it generates without really understanding it. You give the AI the "vibe" of what you want, and it handles the details.

The term comes from how people sometimes use AI coding assistants: describe a feature, hit accept, move on. It works—the code runs—but you haven't learned anything.

**Vibe coding is not inherently bad.** Professional developers sometimes vibe code when prototyping or exploring ideas. But in a learning context, there's a problem: if you don't understand what the AI wrote, you're not building skills you can use later.

## The goal of this assignment

This week, Copilot Agent will write HTML, CSS, and JavaScript for you. **This is intentional.** Agent mode is a legitimate professional tool, and learning to use it effectively is valuable.

But here's the expectation: you should understand the JavaScript code Agent creates. That's why the `/explain` command exists—it turns code you didn't write into code you understand.

## The engagement spectrum

Think of AI-assisted coding as a spectrum:

| Level     | What it looks like                                            | Learning value |
| --------- | ------------------------------------------------------------- | -------------- |
| Pure vibe | Accept without reading                                        | None           |
| Passive   | Read the code but don't investigate                           | Minimal        |
| Active    | Use `/explain`, ask follow-up questions                       | Good           |
| Engaged   | Modify the code, experiment, break things to see what happens | High           |
| Mastery   | Could explain or recreate the core concepts yourself          | Full           |

**Your target for this assignment:**

- **JavaScript**: Active or Engaged level. Use `/explain` and be able to describe what the code does.
- **HTML/CSS**: At least Passive level. Know what's structure (HTML) and what's styling (CSS), but deep understanding isn't required yet.

## What good engagement looks like

### Example: Adding a button

Here's how an engaged student might work with Agent:

**Step 1: Give Agent a task**

> "Add a button that shows an alert when clicked"

Agent creates code in `index.html` and `script.js`.

**Step 2: Read what Agent created**

Don't just click "Accept." Look at the code first. Notice:

- A `<button>` appeared in the HTML
- New JavaScript appeared in `script.js`

**Step 3: Use `/explain` on the JavaScript**

Select the JavaScript code and ask:

> "/explain What does this code do? I'm a beginner."

Copilot will break it down line by line.

**Step 4: Ask follow-up questions**

> "What does addEventListener mean?"
> "What happens if I change 'click' to 'mouseover'?"

**Step 5: Experiment**

Try changing the alert message. Try adding a second button. What breaks? What works?

### Example: When you don't understand something

Agent writes this code:

```javascript
const button = document.querySelector("#myButton");
button.addEventListener("click", () => {
  alert("Hello!");
});
```

You might wonder: "What's the arrow `=>` thing?"

**Good response:** Ask Copilot or use `/explain`. Learn that it's called an "arrow function" and how it works.

**Vibe coding response:** Shrug and accept it. Never think about it again.

The difference matters. Next week, you'll see more arrow functions. Will you recognize them?

## What we're NOT asking you to do

- **Memorize syntax.** You can always look things up.
- **Understand every CSS property.** Focus on JavaScript this week.
- **Avoid using Agent.** Use it! That's the point. Just stay curious about what it creates.
- **Write code from scratch.** Agent is here to help. The skill is learning _from_ what it generates.

## The HTML/CSS exception

This week, it's okay to have only a general sense of the HTML and CSS. If Agent adds this CSS:

```css
button {
  background-color: hsl(210, 60%, 50%);
  border-radius: 4px;
  padding: 0.75rem 1.5rem;
}
```

You should know: "This is styling the button—the color, rounded corners, and spacing." You don't need to memorize what `0.75rem` means.

**JavaScript is different.** When Agent adds this:

```javascript
button.addEventListener("click", () => {
  counter++;
  display.textContent = counter;
});
```

You should use `/explain` and understand:

- `addEventListener` attaches an action to the button
- `counter++` increases a number by one
- `textContent` changes what appears on the page

## Red flags: Signs you're pure vibe coding

Ask yourself these questions:

- Did I accept Agent's changes without reading them?
- Have I used `/explain` at all today?
- Could I describe what my JavaScript does to a classmate?
- Did I ever wonder "why did it do that?" and then investigate?

If you answered "no" to most of these, slow down. You're getting working code but not building understanding.

## Your AI collaboration summary

The summary you submit asks you to reflect on what you learned. This is your accountability mechanism. You need to:

- Describe specific JavaScript concepts you encountered
- Explain in your own words what the code does (don't just copy Copilot's explanation)
- Show evidence of curiosity—questions you asked, things you tried

If you purely vibe coded, you won't have much to write. That's the point.

## A professional perspective

Here's something working developers know: vibe coding has its place. When a developer needs to quickly prototype an idea, they might let AI generate code they don't fully examine. Speed matters; deep understanding can come later.

But that developer already has a foundation. They understand programming concepts well enough to vibe code safely—they can debug problems, recognize when something is wrong, and learn new patterns quickly.

You're building that foundation right now. The point of this assignment isn't to produce a working button—it's to understand how buttons work. Later, you can vibe code all you want. First, build the knowledge base that makes vibe coding safe.

## Summary

| Do this                                 | Not this                        |
| --------------------------------------- | ------------------------------- |
| Use `/explain` on JavaScript            | Accept code without reading it  |
| Ask follow-up questions                 | Assume you understand           |
| Experiment and break things             | Only do the minimum             |
| Paraphrase explanations in your summary | Copy AI text directly           |
| Know generally what HTML/CSS does       | Stress about every CSS property |
| Treat Agent as a teacher                | Treat Agent as a shortcut       |

Agent mode is powerful. Use it to learn, not just to finish.

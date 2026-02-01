# When Agent makes mistakes

Agent is powerful, but it's not perfect. Sometimes the code it creates won't work, or it won't do exactly what you wanted. This is normal—and learning to handle these situations is part of working with AI tools.

## Mistakes are expected

Professional developers who use AI coding assistants expect to iterate. The first attempt rarely works perfectly. This isn't a failure—it's how the process works.

**Your mindset should be:**

- "Let's see what Agent creates"
- "That's close, but I need to adjust it"
- "Something's not working—let me figure out what"

**Not:**

- "It should work perfectly the first time"
- "Agent is broken"
- "I must have done something wrong"

## Common situations and how to handle them

### The code doesn't do anything

**What happened:** You added a button, but clicking it does nothing.

**What to try:**

1. Open the browser's developer console (Right-click → Inspect → Console tab)
2. Look for red error messages
3. Tell Agent what you see:

> "The button doesn't work. The console shows an error: 'Uncaught TypeError: Cannot read property of null'. Can you fix this?"

Or simply:

> "The button doesn't respond when I click it. Can you check the code and fix the issue?"

### It works, but not how you wanted

**What happened:** Agent created something functional, but it's not quite right.

**What to try:**

Be specific about the difference between what you got and what you wanted:

> "The counter works, but it shows the count in an alert. I wanted it to display on the page instead."

> "The button is blue, but I wanted a lighter blue. Can you make it sky blue?"

> "The text appears, but it's below the button. I wanted it above the button."

### Agent changed something you didn't want changed

**What happened:** You asked Agent to add a feature, but it also modified something else.

**What to try:**

1. **Before accepting:** Review all the changes Agent proposes. You can see which files it wants to modify.
2. **If you already accepted:** Ask Agent to undo the unwanted change:

> "You changed the button color when you added the counter. Can you change the button back to blue?"

Or use VS Code's undo feature (`Cmd+Z` / `Ctrl+Z`) to revert changes.

### The page looks broken

**What happened:** After Agent's changes, the layout is messed up or things are in weird places.

**What to try:**

> "The layout looks broken now. The button is overlapping the heading. Can you fix the positioning?"

Agent can usually diagnose CSS issues. If you can describe what looks wrong, it can help fix it.

### You don't understand what Agent did

**What happened:** Agent made changes, and they work, but you have no idea how.

**What to try:**

This is what `/explain` is for:

1. Select the code Agent added
2. Type `/explain`
3. Read the explanation
4. Ask follow-up questions if needed

> "I don't understand what `addEventListener` does. Can you explain it simply?"

## The debugging conversation

Here's what an iterative debugging conversation looks like:

> **You:** "Add a button that shows a greeting when clicked"
>
> **Agent:** _Creates code_
>
> **You:** _Tests it_ "Nothing happens when I click the button"
>
> **Agent:** "Let me check... I see the issue. The script is loading before the button exists in the DOM. Let me move the script tag or add a DOMContentLoaded listener."
>
> **Agent:** _Fixes the code_
>
> **You:** _Tests again_ "Now it works! But the greeting shows in an alert. Can you make it appear on the page instead?"
>
> **Agent:** _Modifies to use textContent instead of alert_
>
> **You:** "Perfect, that's what I wanted."

Notice the pattern: test → report what happened → let Agent fix it → test again.

## When to start over

Sometimes it's easier to start fresh than to fix a tangled mess:

> "This has gotten complicated. Can you remove all the JavaScript from script.js and start over? I want a simple button that counts clicks and shows the count on the page."

Starting over isn't giving up—it's a practical choice when the code has become hard to follow.

## Checking your work

After Agent makes changes, always:

1. **Save all files** (auto-save should handle this)
2. **Refresh the browser** (or let Live Server do it)
3. **Test the feature** by actually clicking, typing, or interacting
4. **Check the console** for errors (Right-click → Inspect → Console)

If you skip testing, you won't know if something is broken until later—when it's harder to figure out what went wrong.

## Using the browser console

The browser console is your friend. It shows JavaScript errors that explain why things aren't working.

**How to open it:**

1. Right-click anywhere on your page
2. Select "Inspect" (or "Inspect Element")
3. Click the "Console" tab

**What to look for:**

- Red text = errors (something is broken)
- Yellow text = warnings (might be a problem)
- Regular text = console.log output (helpful for debugging)

**Common errors you might see:**

| Error                          | What it usually means                                 |
| ------------------------------ | ----------------------------------------------------- |
| "Cannot read property of null" | JavaScript tried to use an element that doesn't exist |
| "Unexpected token"             | Syntax error—maybe a missing bracket or quote         |
| "is not defined"               | A variable or function name is misspelled             |

You don't need to understand these fully—just copy the error message and share it with Agent.

## Frustration is normal

If you're feeling frustrated:

1. **Take a breath.** This happens to everyone, including professionals.
2. **Re-read your prompt.** Was it clear? Could Agent have misunderstood?
3. **Start smaller.** Ask for one simple thing instead of a complex feature.
4. **Ask Agent to explain.** Sometimes understanding the problem helps solve it.

Working with AI tools has a learning curve. Each mistake teaches you something about how to communicate more effectively.

## Summary

- Expect to iterate—first attempts rarely work perfectly
- Describe problems clearly: what you expected vs. what happened
- Check the browser console for error messages
- Use `/explain` when you don't understand what Agent did
- Starting over is sometimes the right choice
- Test after every change
- Frustration is normal; it gets easier with practice

# Writing prompts for Agent

Getting good results from Copilot Agent starts with how you ask. This guide shows you how to write prompts that help Agent understand what you want.

## The basics: Be specific

Agent works best when you tell it exactly what you want. Compare these prompts:

| Vague prompt          | Specific prompt                                                     |
| --------------------- | ------------------------------------------------------------------- |
| "Add a button"        | "Add a button that shows an alert saying 'Hello!' when clicked"     |
| "Make it look better" | "Make the button blue with white text and rounded corners"          |
| "Add some JavaScript" | "Add a counter that increases by 1 each time the button is clicked" |

The specific prompts give Agent clear direction. The vague prompts leave Agent guessing—and it might guess wrong.

## The anatomy of a good prompt

A helpful prompt often includes:

1. **What** you want (the feature or change)
2. **Where** it should go (if not obvious)
3. **How** it should behave (the details)

**Example:**

> "Add a text input field above the button. When the user types their name and clicks the button, show an alert that says 'Hello, [name]!'"

This prompt tells Agent:

- **What**: A text input field and modified button behavior
- **Where**: Above the button
- **How**: Combines the input value with a greeting in an alert

## Start simple, then refine

You don't need to describe everything in one prompt. It's often better to:

1. Start with a basic request
2. See what Agent creates
3. Ask for adjustments

**Example conversation:**

> **You:** "Add a button that counts clicks"
>
> **Agent:** _Creates a button with a counter_
>
> **You:** "Show the count on the page instead of in an alert"
>
> **Agent:** _Modifies to display count in a paragraph_
>
> **You:** "Add a reset button that sets the count back to zero"
>
> **Agent:** _Adds a second button_

This iterative approach is how professionals work with AI tools. You don't need to think of everything upfront.

## Prompts for common Week 2 tasks

### Adding interactive elements

```text
Add a button with the text "Click me" that shows an alert saying "Hello!" when clicked.
```

```text
Add a text input field where users can type their name.
```

```text
Add a counter that displays on the page and increases each time a button is clicked.
```

### Styling elements

```text
Make the button blue with white text.
```

```text
Add some spacing between the button and the paragraph above it.
```

```text
Center all the content on the page.
```

### Connecting elements

```text
When the user types in the input field and clicks the button, display what they typed below the button.
```

```text
Add a second button that resets the counter to zero.
```

```text
Make the heading change color when the button is clicked.
```

## What to avoid

### Too vague

> "Make it work"

Agent doesn't know what "it" is or what "work" means to you.

### Too complex all at once

> "Create a full shopping cart with product images, quantities, prices, a total calculator, discount codes, and checkout functionality"

This is too much for one prompt. Break it into smaller pieces.

### Assuming Agent knows your intent

> "Fix the thing"

Agent doesn't know what's broken or what you expected to happen.

**Better:** "The button doesn't show an alert when I click it. Can you check the JavaScript and fix the issue?"

## When Agent asks questions

Sometimes Agent will ask for clarification:

> "Do you want the counter to start at 0 or 1?"
> "Should the alert include the user's name?"
> "Where would you like me to place the new button?"

This is good! Answer the questions, and Agent will have a better understanding of what you want.

## Describing what's wrong

When something isn't working, describe:

1. **What you expected** to happen
2. **What actually happened** (or didn't happen)
3. **When** it happens (on click, on page load, etc.)

**Example:**

> "When I click the button, nothing happens. I expected to see an alert with my name, but the page just sits there."

This gives Agent the information it needs to diagnose the problem.

## The feedback loop

Working with Agent is a conversation, not a one-shot request. The pattern is:

1. **Prompt** → Ask for something
2. **Review** → Look at what Agent created
3. **Refine** → Ask for adjustments or move to the next feature
4. **Repeat**

Each cycle teaches you more about how to communicate with AI tools effectively.

## Practice prompts

Try these prompts with Agent and see what happens:

1. "Add a button that changes color each time it's clicked"
2. "Create a simple form with a name field and a submit button"
3. "Add a paragraph that shows the current date and time"
4. "Make the page background change to a random color when a button is clicked"

After each one, use `/explain` to understand the JavaScript Agent created.

## Summary

- Be specific about what you want, where, and how
- Start simple and refine through conversation
- Describe problems clearly: expected vs. actual behavior
- Answer Agent's questions to help it understand your intent
- Iterate—you don't need to get it perfect on the first try

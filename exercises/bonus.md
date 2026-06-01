# Bonus Exercises

## The "Spec Template" (spec.md)

This is for the person who says, "I don't know what to write." It uses a "Fill-in-the-Blanks" approach.

```
# Project: [Name of your App]

## 🎯 The "Vibe" (Goal)
I want to build a [Simple description, e.g., Task Tracker] that helps me [Primary benefit]. It should feel [Minimalist / Professional / Fun].

## 🛠️ Tech Stack
- **Language:** TypeScript
- **Runtime:** Node.js
- **Storage:** Local JSON file (no database setup needed)

## 🏗️ Core Features (The "Must-Haves")
- [ ] Feature 1: (e.g., I can add a task with a title and a priority)
- [ ] Feature 2: (e.g., I can list all tasks in a table format)
- [ ] Feature 3: (e.g., I can mark a task as "Done")

## ⛔ Constraints (The "Guardrails")
- Don't use any external CSS libraries; keep it CLI-based or use basic HTML.
- Always validate that the task title isn't empty before saving.
- If the JSON file doesn't exist, create it automatically on start.
```

## The "Cheat Sheet": Context Engineering

Hand this out as a physical card or a pinned message in your workshop chat.

🌶️ Context Engineering Cheat Sheet - Techniques

### Persona

- **What to say:** "Act as a Senior Backend Engineer who loves clean, DRY code."
- **Why it works:** Sets a high quality bar and dictates the architectural style.

### The "Why"

- **What to say:** "I am building this for a workshop; keep the code beginner-friendly."
- **Why it works:** Prevents the AI from over-engineering or using overly complex libraries.

### Format Fix

- **What to say:** "Output only the code block. No explanations or conversational filler."
- **Why it works:** Saves time, tokens, and makes the response easier to copy-paste.

### Fenced Rules

- **What to say:** "Rules: [1. No classes, only functions. 2. Use 'const' only.]"
- **Why it works:** Creates hard guardrails to enforce your specific coding standards.

### The Anchor

- **What to say:** "@file.ts - Refactor this to use the logic found in @utils.ts"
- **Why it works:** Uses the @ symbol to pin specific files, ensuring the AI has the right context.

```
[ IDEATION ]
            |
            v
     +--------------+
     |   SPEC.MD    | <--- Define the "Vibe"
     +--------------+
            |
            | (The Anchor)
            v
     +--------------+
     |  OPEN CODE   | <--- The AI Agent
     +--------------+
      ^     |      |
      |     |      | (The Rules)
      |     v      |
      |  [ CODE ]  | <--- Working Software
      |     |      |
      +-----+------+ 
        Iterate!
```

## The "Goldilocks" App Example

An app that isn't too hard, but "spicy" enough to show off AI capabilities.

### The Project: "The Mood-Based Recipe Suggester"

- The Concept: A small app where a user types in their current mood (e.g., "Tired," "Celebratory," "Lazy") and the app suggests a 3-ingredient recipe.
- Why it's perfect for a workshop:
  - Logic: It requires a simple data structure (an object or JSON map of moods to recipes).
  - Agentic Power: Participants can ask OpenCode to "Go find 5 quick recipes for someone feeling 'Lazy' and add them to my data file."
  - Extension: It’s easy to make "Spicy" by adding a feature that exports the recipe to a .txt file or adds a "Randomize" button.
- Prompt to start: "OpenCode, help me initialize a TypeScript project for a Mood-Based Recipe Suggester. Use the spec.md in this folder as your guide."

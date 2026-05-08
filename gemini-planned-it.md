# 🌶️ Workshop Outline: Getting Spicy with Vibe Coding

## Part 1: The Vibe Shift (20 Minutes)
Generated slides at: https://docs.google.com/presentation/d/1Tg1HH8_x1grtkq6wY5iy2Tcr0yASMg-TG6fRn1YRbIM/preview?slide=id.p1

- The Concept: Briefly explain the transition from "Syntax-First" to "Intent-First" development.

- Spec-Driven Development: Why writing a spec is faster than writing a bug. Show a "Bad Prompt" vs. a "Spicy Spec" (Context, Constraints, and Outcome).

- Demo: A 5-minute "Speed Build." Use Open Code to generate a small, functional utility (e.g., a CLI tool that summarizes local Markdown files) to show the audience what "Vibe Coding" looks like in real-time.

## Part 2: Context Engineering & The "Recipe" (30 Minutes)
- Activity: Participants choose a small project idea (or use a provided prompt like a "Personal Habit Tracker CLI" or a "Markdown-to-HTML Blog Converter").

- Task: Instead of coding, they must write a Specification Document (spec.md).
    - Inputs: Tech stack (TypeScript/Node), file structures, and data types.
    - Constraints: No external databases (use local JSON), strict error handling.
    - Step-by-Step: Break the logic down into three distinct phases.

## Part 3: Hands-On: Delegating to the Agent (70 Minutes)
### Phase 1: Foundation (20 mins)

- Action: Use Open Code to initialize the project structure and the primary data models based on your spec.md.
- Goal: Get a "Hello World" version of your app running where the basic data structure exists.

### Phase 2: Logic Implementation (20 mins)

- Action: Use the Anchor technique to point the agent at your foundation and ask it to build the core "Must-Have" features from your spec.
- Goal: Move from a folder structure to a functional app that actually does the primary task (e.g., saving a recipe or a task).

### Phase 3: The "Spicy" Pivot (20 mins)

- Action: Add a "Spicy" feature that wasn't in the original plan (e.g., adding a search filter, a "Randomize" button, or exporting to a file).
- Goal: Learn to steer the AI. This is where participants practice "Context Engineering" when the agent starts to drift or get confused by the new requirements.

### Phase 4: Polish & Vibe Check (10 mins)

- Action: Ask the agent to refactor for readability or add "beginner-friendly" comments.
- Goal: Ensure the code is clean and matches the "Persona" you set in the cheat sheet.

Troubleshooting: Mentors walk the floor, helping users "re-contextualize" the AI when the "vibe" gets messy.


---
## Part 3 (Newbie-friendly): Hands-On: Delegating to the Agent (70 Minutes)
### Phase 1: Setting the Kitchen (20 mins)
- The Idea: You don't start cooking by throwing food in a pan; you get your tools out first.
- The Action: Tell the AI, "Set up a new folder for my project and create a blank list where I can store my data."
- The Goal: Getting the "skeleton" of the app ready so it has a place to live.

### Phase 2: Cooking the Main Dish (20 mins)
- The Idea: Now we follow the recipe you wrote in your spec.md.
- The Action: Ask the AI to build the #1 most important thing. If it’s a recipe app, ask it to "Make a button that lets me save a new recipe."
- The Goal: Getting the app to actually work for the first time.

### Phase 3: Adding the Spice (20 mins)
- The Idea: Every good dish needs a little extra kick. This is where you get creative.
- The Action: Ask for a "surprise" feature. "Now, make the app suggest a random recipe if I’m feeling indecisive."
- The Goal: Learning how to talk to the AI when you want to change the plan. This is where you practice being a "Chef" (the boss) and the AI is your "Sous-Chef" (the helper).

### Phase 4: Cleaning Up (10 mins)
- The Idea: A good chef never leaves a messy kitchen.
- The Action: Ask the AI to "Explain this code to me like I’m five" and "Make the code look neat and professional."
- The Goal: Making sure you actually understand what was built, so it’s not just "magic" to you.

### 💡 Two Simple Rules for Beginners
1. Talk to it like a person: Don't worry about "code talk." If it makes a mistake, just say "That didn't work, it gave me an error that said X. Can you try a different way?"
2. One thing at a time: Don't ask it to build the whole app at once. Ask for the "Foundation," then one "Feature," then the "Spice." If you give it too much at once, the "vibe" gets messy!


---

## Part 4: The Spicy Showcase & Retrospective (30 Minutes)
The "Vibe Check": A few volunteers show what they built and, more importantly, how they prompted to get there.

Discussion: What was harder than expected? When did the AI hallucinate, and how did a better spec fix it?

Closing: Resources for further exploration (Open Source agents, prompt libraries).

---


### Recommended "Spicy" Project Ideas for Attendees:
- The "Daily Standup" Bot: A script that parses a Git log for the last 24 hours and formats it into a Slack-ready update.
- Image Metadata Organizer: A tool that reads a folder of images and renames them based on their creation date and dimensions.
- Local Knowledge Base Search: A tool that uses fzf logic to search through a directory of Markdown notes.

---

### Pre-Workshop Checklist:

[ ] Send out a "Spec Template" .md file to participants.

[ ] Ensure everyone has an API key (if required by the local setup of Open Code).

[ ] Prepare a "Cheat Sheet" of common Context Engineering keywords (e.g., "Act as...", "Strictly follow...", "Output only code").

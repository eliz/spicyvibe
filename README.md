# spicyvibe

1. OpenCode Setup GuideOpenCode (opencode.ai) is a terminal-based agent. Since it’s 2026, the installation is streamlined, but users often trip up on API keys.  Step-by-Step for Attendees:Terminal Check: Open your terminal (VSCode integrated terminal is best).  Install: Run the one-command installer:curl -fsSL [https://opencode.ai/install](https://opencode.ai/install) | bashConnect AI: Run /connect in your terminal.Pro Tip: For the workshop, recommend OpenCode Zen. It’s a pre-configured, curated model list that doesn't require individual OpenAI/Anthropic keys—great for a group setting.  Authorize: Follow the link to opencode.ai/auth to sign in and grab your session token.Initialize Project: Navigate to your project folder and run opencode /init. This creates an AGENTS.md file, which is the "brain" OpenCode uses to understand your specific codebase.2. The "Spec Template" (spec.md)This is for the person who says, "I don't know what to write." It uses a "Fill-in-the-Blanks" approach.Markdown# Project: [Name of your App]

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
3. The "Cheat Sheet": Context EngineeringHand this out as a physical card or a pinned message in your workshop chat.TechniqueWhat to say to the AIWhy it worksPersona"Act as a Senior Backend Engineer who loves clean, dry code."Sets the quality bar.The "Why""I am building this for a workshop, keep the code beginner-friendly."Prevents over-engineering.Format Fix"Output only the code block. No explanations."Saves time and tokens.Fenced Rules"Rules: [1. No classes, only functions. 2. Use 'const' only.]"Enforces your specific style.The Anchor"@file.ts - Refactor this to use the logic found in @utils.ts"Uses @ to point the AI to specific context.4. The "Goldilocks" App ExampleAn app that isn't too hard, but "spicy" enough to show off AI capabilities.The Project: "The Mood-Based Recipe Suggester"The Concept: A small app where a user types in their current mood (e.g., "Tired," "Celebratory," "Lazy") and the app suggests a 3-ingredient recipe.Why it's perfect for a workshop:Logic: It requires a simple data structure (an object or JSON map of moods to recipes).Agentic Power: Participants can ask OpenCode to "Go find 5 quick recipes for someone feeling 'Lazy' and add them to my data file."Extension: It’s easy to make "Spicy" by adding a feature that exports the recipe to a .txt file or adds a "Randomize" button.Prompt to start: "OpenCode, help me initialize a TypeScript project for a Mood-Based Recipe Suggester. Use the spec.md in this folder as your guide."

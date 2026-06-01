# spicyvibe

## OpenCode Setup Guide

OpenCode (opencode.ai) is a terminal-based agent. Since it’s 2026, the installation is streamlined, but users often trip up on API keys.

1. Terminal Check: Open your terminal (Can also use VSCode integrated terminal).

2. Install: Run the one-command installer:

    ```
    curl -fsSL [https://opencode.ai/install](https://opencode.ai/install) | bash
    ```

    > If you have issues, visit this URL: <https://opencode.ai/docs/#install> and follow the instructions for  installing in your laptop.

3. You should also install the following coding software as well:

    - [VSCode](https://code.visualstudio.com/)
    - [Git](https://git-scm.com/)

## Exercises

1. [Exercise 1: Configure OpenCode](./exercises/exercise1.md)
2. [Exercise 2: Writing code with Plan Mode](./exercises/exercise2.md)
3. Exercise 3: Spec Driven Development:
    - [Using OpenSpec](./exercises/exercise3a.md) (Requires NodeJS)
    - [Using SpecKit](./exercises/exercise3a.md) (Requires Python)
4. [Bonus Exercises](./exercises/bonus.md)

## Some Extra Advice

### 1. Manage your context window

As you use OpenCode, be mindful of the how much of the [Context Window](https://www.datacamp.com/blog/context-window). The context window of Free models fills up very fast. So be mindful of how many % your tokens have taken up.

> **Pro-Tip:**
> 1. Use the `/compact` command to do some garbage collection.
> 2. Sometimes it might make more sense to start a new session altogether and continue from where you left off.

### 2. Not all models are the same

Some LLM models are better at Thinking. Others are better at execution. In today's exercise, we are just using the free models, so we might not experience the full potential of these more expensive models. But chances are, the more expensive models can think & plan faster.

> **Pro-Tip:**
> 1. Use the better (and more expensive) models for the planning phase and 
> 2. Switch to a cheaper model for the implementation phase.

### 3. Use version control

After every important milestone, it makes sense to just make a Git commit to preserve a snapshot of the code changes. If anything breaks badly, you can still revert to the last known good state.

### 4. Secure coding habits

Create a `.gitignore` file to ensure that you don't accidentally commit sensitive files to Git.

- Do not commit your `.env`
- Ignore `node_modules` to keep your git commit small.
- Maybe use the Coding Agent to suggest an approriate list of files to add to your `.gitignore` file based on your project folder format.
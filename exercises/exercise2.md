# Exercise 2: Do some planning

1. After installing OpenCode, open your terminal and change to your working directory (you can create a new folder too).

    ```bash
    cd ~
    mkdir -p workspace/vibecode1
    cd workspace/vibecode1
    ```

2. Type `opencode` to start the OpenCode TUI.

3. Initialize Project: Navigate to your project folder and run opencode `/init`. This creates an AGENTS.md file, which is the "brain" OpenCode uses to understand your specific codebase.

## Plan Mode

OpenCode has a *Plan mode* that disables its ability to make changes and instead suggest how it’ll implement the feature.

1. Press the `<tab>` key to enter *Plan Mode*.

2. Let's try to build a simple tic tac toe game.

    Copy and paste this into your OpenCode chat box:

    ```
    I want to build a simple Tic Tac Toe game that runs in the terminal.

    Before writing any code:

    1. Define the requirements and game rules.
    2. Identify the main components and data structures needed.
    3. Describe the game flow from start to finish.
    4. List the functions/classes that should be implemented and their responsibilities.
    5. Identify edge cases and error handling requirements.
    6. Propose a simple project structure.
    7. Create an implementation plan broken into small, testable steps.

    Keep the design simple and suitable for a beginner developer. Do not generate code yet—focus only on planning and architecture.
    ```

3. Follow the on screen instructions and let's see what it builds.

4. You can chat and discuss changes if you don't agree with anything that was suggested.

5. Remember to exit *Plan Mode* before executing (press `<tab>` key again).

    Copy and paste this into your OpenCode chat box:
    
    ```
    Let's go
    ```

6. Use VScode to see what's being added to the folder.

7. Can proceed to play the game in terminal (you can open a new terminal tab).

8. You can exit the OpenCode by typing: `exit` and press `<enter>`.

    > **Pro-Tip:** Notice that you can get back into the same session with the command shown on screen.
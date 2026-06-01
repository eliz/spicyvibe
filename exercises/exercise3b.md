# Exercise 3: Spec Driven Development (SpecKit)

1. Let's create a new project folder & `cd` into the new project folder:

    ```bash
    cd ~
    mkdir -p workspace/vibecode2
    cd workspace/vibecode2
    ```

2. Initialize Git in this folder:

    ```bash
    git init
    ```

3. Let's install [SpecKit](https://github.com/github/spec-kit).

    ```bash
    uv tool install specify-cli --from git+https://github.com/github/spec-kit.git@v0.8.18
    ```

4. Initialize SpecKit in the project folder:

    ```bash
    specify init --here
    ```

5. Select **OpenCode** as the coding agent integration.

    - Press `<up>` or `<down>` key to find `opencode`. 
    - Press `<enter>` to confirm the selection.

6. Select your script type (`sh` for bash/zsh or `ps` for PowerShell)

7. Start **OpenCode** from this project folder.

8. Use this prompt to establish project principles:

    ```
    /speckit.constitution Create principles focused on code quality, testing standards, user experience consistency, and performance requirements
    ```

    You can see the Constitution file here: `.specify/memory/constitution.md`

9. Use this prompt to establish what you want to build:

    ```
    /speckit.specify Build a small web app where a user types in their current mood (e.g., 'Tired', 'Celebratory', 'Lazy') and the app suggests a 3-ingredient recipe.
    ```

8. Review the artifacts in the `specs/001-mood-recipe` folder. Use VSCode to open the project folder to review the changes.

9. Chances are, the proposal does not include an image of the recipe.

    ```
    I would like to include a photo of the recipe in the display page.
    ```

10. Use the `/speckit.plan` command to provide your tech stack and architecture choices.

    ```
    /speckit.plan The application uses FastAPI with minimal number of libraries. Use vanilla HTML, CSS, and JavaScript as much as possible. Use images from Unsplash and metadata is stored in a local JSON database.
    ```

11. Review the new artifacts in `specs/001-mood-recipe` folder. Use VSCode to open the project folder to review the changes.

12. Run `/speckit.tasks` to start preparing the tasks.

13. Run `/speckit.implement` to start implementing.

12. Test out the app in a separate terminal.

    Follow the instructions in `specs/001-mood-recipe/quickstart.md`:

    ```bash
    cd backend
    uvicorn app.main:app --reload --port 8000
    ```

    Open browser to <http://localhost:8000>.


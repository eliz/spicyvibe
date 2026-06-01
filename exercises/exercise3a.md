# Exercise 3: Spec Driven Development (OpenSpec)

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

3. Let's install [OpenSpec](https://github.com/Fission-AI/OpenSpec/).

    ```bash
    npm install -g @fission-ai/openspec@latest
    ```

4. Initialize OpenSpec in this project folder:

    ```bash
    openspec init
    ```

5. Select **OpenCode** as the tool.

    - Press `<up>` or `<down>` key to find `OpenCode`. 
    - Press `<space>` key to select the tool. 
    - Press `<enter>` to confirm the selection.

6. Start **OpenCode** from this project folder.

7. Use this prompt:

    ```
    /opsx-propose "Build a small web app where a user types in their current mood (e.g., 'Tired', 'Celebratory', 'Lazy') and the app suggests a 3-ingredient recipe."
    ```

8. Review the artifacts in the `openspec` folder. Use VSCode to open the project folder to review the changes.

9. Chances are, the proposal does not include an image of the recipe.

    ```
    I would like to include a photo of the recipe in the display page.
    ```

10. Once you are happy with the proposal, type: `/opsx:apply` to start the implementation.

11. Sometimes things might stall. Just press `<esc>` twice and type: `continue` and press `<enter>` to continue where it hung.

12. Test out the app in a separate terminal.

    ```bash
    npm start
    ```

13. If there are bugs or you have ideas to enhance things, just type in the statement into OpenCode:

    ```
    The images are not showing in the web page
    The loading spinner and text "Cooking up an idea..." is still showing after i get a recipe.
    Shall we use recipe photos from Unsplash?
    ```

    And see how it fixes the problem or enhance the app.

14. Once you are happy, can archive the work:

    ```
    /opsx:archive
    ```

## Troubleshooting:


If things get stuck, might be due to the application server running in the background.

```
pa aux | grep node
```

Find the process number and kill it:

```
kill -9 1234455
```
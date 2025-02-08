I want you to review the entire diff from what is currently queued for changes with git. You should also look at the status of all files. Sometimes we just add or remove files. Make sure to run all git commands so that they don't paginate. Use `git --no-pager diff` to view the changes. Sometimes it will be empty and that is okay. Then, I want you to create isolated patch commits of similar concepts so that each commit is nice and clean and revertable based on a single concept. No giant single commits of unrelated concepts. Create nice coherent git messages and try to explain "why" instead of what the code is doing in the git messages. Some changes may cross multiple files and yet be part of the same concept. Perform patch commits in these cases using the cli, but make sure the cli does not prompt the user for interaction. I like git messages like this:

Summary under 50 chars

- Bullet point 1
- Bullet point 2
- etc

Use as many bullet boints as necessary to articular clearly what each commit was intended to do. Again, focus on why we might be making these changes when possible

Here are the steps to follow:

1. Review the changes:
    ```sh
    git status -s
    git --no-pager diff
    ```

2. Stage the changes for a specific concept:
    ```sh
    git add <file1> <file2> ...
    ```

3. Commit the changes with a meaningful message:
    ```sh
    git commit -m "Summary under 50 chars

    - Bullet point 1
    - Bullet point 2"
    ```

4. Repeat steps 2 and 3 for each concept until all changes are committed.

Make sure to run all commands without requiring user interaction. Use the `-y` flag where applicable to automatically confirm prompts.

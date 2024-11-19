# Task 4: Rebasing

## Objective
Learn how to use `git rebase` to update your feature branch with the latest changes from `main`.

## Scenario
Imagine you’ve been working on a feature branch, but in the meantime, changes have been made to the `main` branch. Instead of merging `main` into your branch, you’ll rebase your feature branch on top of `main`.

## Steps
1. **Ensure your `main` branch is up to date**:
   - First, ensure you’re on the `main` branch:
     ```bash
     git checkout main
     ```
   - Pull the latest changes from `main`:
     ```bash
     git pull origin main
     ```

2. **Switch to your feature branch**:
   - Now switch to your `feature-branch` (the branch you’ve been working on):
     ```bash
     git checkout feature-branch
     ```

3. **Rebase your feature branch onto `main`**:
   - Apply your feature branch’s commits on top of the updated `main` branch:
     ```bash
     git rebase main
     ```

4. **Handle any conflicts**:
   - If there are any conflicts, Git will pause and ask you to resolve them. Open the conflicting files and resolve the issues.
   - After resolving conflicts, use:
     ```bash
     git add <resolved-file>
     git rebase --continue
     ```

5. **Push the rebased branch**:
   - After a successful rebase, you’ll need to force push your branch because the history has been rewritten:
     ```bash
     git push origin feature-branch --force
     ```

## Next Steps
Proceed to [Task 5: Creating Pull Requests](task5.md).

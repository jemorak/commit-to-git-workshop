# Task 5: Creating Pull Requests

## Objective
Learn how to create a pull request (PR) to propose changes from your feature branch to `main`.

## Scenario
After working on your feature, you need to submit it for review. A pull request (PR) is a way to notify the repository maintainers about the changes you’ve made and request that those changes be merged into the `main` branch.

## Steps
1. **Push your changes to your fork** (if you haven't already):
   - Ensure you have pushed your `feature-branch` to your fork:
     ```bash
     git push origin feature-branch
     ```

2. **Go to your GitHub repository**:
   - Open your forked repository on GitHub.
   - GitHub will usually show a prompt to "Compare & pull request" when you push to a branch. Click on that button.

3. **Create a pull request**:
   - Title the pull request (e.g., "Add feature-branch changes").
   - Add a description summarizing the changes you made.
   - Make sure the base branch is `main` and the compare branch is `feature-branch`.
   - Click on "Create pull request".

4. **Review the pull request**:
   - Once the PR is created, review your changes, and make sure everything looks correct.
   - You may request a review from someone else if you're working in a team, or you can just merge it yourself if you're working alone.

5. **Merge the pull request**:
   - After reviewing, if everything is okay, click on "Merge pull request" and then confirm.
   - This will merge your feature branch into the `main` branch.

## Congratulations! You’ve completed the tutorial!

Your feature is now part of the main branch!

---

### **Additional Step: Clean Up**

After the PR is merged, you can delete your feature branch:
```bash
git branch -d feature-branch  # Delete the local branch
git push origin --delete feature-branch  # Delete the remote branch

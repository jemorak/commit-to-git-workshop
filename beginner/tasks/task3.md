
# Task 3: Resolving Merge Conflicts

## Objective
Learn how to resolve merge conflicts when merging branches.

## Steps
1. **Create a conflict:**
   - On `feature-branch`, edit `conflict-file.txt` and add:
     ```
     Feature branch change
     ```
   - Commit the change:
     ```bash
     git commit -m "Feature branch change"
     ```

   - Switch to `main` and make a conflicting edit:
     ```bash
     git checkout main
     echo "Main branch change" >> conflict-file.txt
     git commit -am "Main branch change"
     ```

2. **Merge and resolve the conflict**:
   - Merge `feature-branch` into `main`:
     ```bash
     git merge feature-branch
     ```
   - Resolve the conflict in `conflict-file.txt`.

3. **Commit the resolution:**
   ```bash
   git add conflict-file.txt
   git commit -m "Resolve merge conflict"

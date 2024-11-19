# Task 2: Creating and Pushing Branches

## Objective
Learn how to create a new branch, make changes, and push it to GitHub.

## Steps
1. **Create a new branch**:
   ```bash
   git checkout -b feature-branch

2. **Make changes**:
   
   Open `file1.txt` and make a random change:

      ```text
      Hello from feature-branch!
      ```

   Open `file2.txt` and add a note:

   ```text
   Editing this file as part of Task 2!
   
3. **Add and commit your changes:**

   ```bash
   git add example-file1.txt example-file2.txt
   git commit -m "Add a change from feature-branch"

4. **Push the branch:**
   ```
   git push origin feature-branch
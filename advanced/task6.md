# GitHub Actions and GitHub Pages Tasks

## Task 6: Automate with GitHub Actions

### Objective
Set up a GitHub Actions workflow to automate your project. The workflow should:
1. Run tests to ensure the code is functional.
2. Deploy the project to GitHub Pages.

### Steps
1. **Create a Workflow**:
   - Add a file named `.github/workflows/ci.yml` in your repository.
   - Define a CI/CD pipeline that:
     - Checks out the repository.
     - Runs any tests or builds.
     - Deploys the project to GitHub Pages.

   Example workflow:
   ```yaml
   name: CI/CD Pipeline

   on:
     push:
       branches:
         - main
     pull_request:
       branches:
         - main

   jobs:
     build-and-deploy:
       name: Build and Deploy
       runs-on: ubuntu-latest

       steps:
         - name: Checkout code
           uses: actions/checkout@v3

         - name: Set up Node.js
           uses: actions/setup-node@v3
           with:
             node-version: '16'

         - name: Install dependencies and build
           run: |
             npm install
             npm run build

         - name: Deploy to GitHub Pages
           uses: peaceiris/actions-gh-pages@v3
           with:
             github_token: ${{ secrets.GITHUB_TOKEN }}
             publish_dir: ./build

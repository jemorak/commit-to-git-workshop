# Task 7: Deploy with GitHub Pages

## Objective
Host your project live using GitHub Pages, making it accessible to anyone with a URL.

---

## Instructions

### Step 1: Enable GitHub Pages
1. Go to your repository on GitHub.
2. Navigate to **Settings > Pages**.
3. Under **Source**, select the `main` branch.
4. Choose either:
   - **Root** directory: Use the top-level directory.
   - **/docs** folder: Use a `docs` folder in the repository.
5. Save your settings. A deployment URL will be generated (e.g., `https://username.github.io/repository-name`).

---

### Step 2: Prepare Your Project
1. Add a simple HTML file to the repository:
   - Create an `index.html` file:
     ```html
     <!DOCTYPE html>
     <html>
     <head>
       <title>My GitHub Pages Project</title>
     </head>
     <body>
       <h1>Welcome to My Live Site!</h1>
       <p>This project is hosted using GitHub Pages.</p>
     </body>
     </html>
     ```

2. Push this file to the branch you configured in Step 1.

---

### Step 3: Deploy and Access
1. After pushing, GitHub Pages will automatically deploy your project.
2. Wait a few minutes for the deployment to complete.
3. Access your live site at the provided URL under **Settings > Pages**.

---

## Challenge
1. Add a `style.css` file to style your page:
   - Example:
     ```css
     body {
       font-family: Arial, sans-serif;
       text-align: center;
       background-color: #f4f4f9;
     }

     h1 {
       color: #333;
     }
     ```
   - Link it to your `index.html` file:
     ```html
     <link rel="stylesheet" href="style.css">
     ```

2. Create a `docs/index.md` file for documentation and configure GitHub Pages to use the `/docs` folder:
   - Example `index.md` content

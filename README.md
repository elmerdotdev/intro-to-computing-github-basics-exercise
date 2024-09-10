# Git Basics Exercise

## Objective

Learn how to track changes with `git add`, commit changes with `git commit`, and upload your code to a remote repository using `git push`.

## Prerequisites

- Make sure you have Git installed on your machine.
- Ensure you have a GitHub (or any Git hosting service) account.

## Step-by-Step Instructions

### 1. Create a New Local Git Repository

1. Open your terminal.
2. Navigate to a folder where you want to create your project.
3. Run the following commands:

   ```bash
   mkdir git-exercise
   cd git-exercise
   git init
   ```

### 2. Create a New File

1. Inside your `git-exercise` folder, create a new file called `index.html`:

   ```bash
   touch index.html
   ```

2. Open `index.html` in any text editor and add the following content:

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Git Exercise</title>
   </head>
   <body>
       <h1>Hello, Git!</h1>
   </body>
   </html>
   ```

### 3. Stage Your Changes with `git add`

1. In the terminal, check the status of your repository:

   ```bash
   git status
   ```

2. Stage the new file with the following command:

   ```bash
   git add index.html
   ```

3. Verify the file was staged:

   ```bash
   git status
   ```

### 4. Commit Your Changes with `git commit`

1. Commit the staged file with a message:

   ```bash
   git commit -m "Initial commit - added index.html"
   ```

### 5. Push to a Remote Repository with `git push`

1. Go to GitHub (or your Git hosting service) and create a new repository. **Do not initialize the repository with a README**. After creating the repository, copy the HTTPS url.
2. In your terminal, link your local repository to the remote one:

   ```bash
   git remote add origin https://github.com/your-username/git-exercise.git # Make sure to change the URL to the HTTPS URL you copied from GitHub
   ```

3. Push your code to the remote repository:

   ```bash
   git push -u origin master
   ```

### 6. Verify Your Work

1. Go to your remote repository (on GitHub) and refresh the page.
2. You should now see your `index.html` file.

## Extra Challenge

1. Modify the content of `index.html` (e.g., change the heading text to something else).
2. Stage, commit, and push the changes to the remote repository.

   ```bash
   git add index.html
   git commit -m "Updated heading text"
   git push
   ```

Congratulations! You’ve completed the Git basics exercise.

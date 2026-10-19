# My Study Planner — ISE-2

## Project objective
My Study Planner is a simple website that lets students add study tasks, mark them done, and delete tasks.

## Technology used
- HTML
- CSS
- JavaScript
- Git and GitHub
- Jenkins

## How to run
1. Download or clone this repository.
2. Open `index.html` in a web browser.
3. Enter a task, choose a subject, and click **Add Task**.
4. Use **Done** to mark a task complete or **Delete** to remove it.

## Suggested five meaningful changes
Make and commit these changes one at a time. Only write that you completed a change after you have actually done it.

1. Create the page title and header — `git commit -m "Create study planner homepage"`
2. Add CSS styling — `git commit -m "Style study planner page"`
3. Add task creation — `git commit -m "Add new study tasks"`
4. Add Done and Delete buttons — `git commit -m "Add task completion and deletion"`
5. Add task count and empty message — `git commit -m "Show task count and empty state"`

## Git and GitHub
Create an empty GitHub repository, then run these commands in this folder. Replace the URL with your own repository URL.

```bash
git init
git add .
git commit -m "Create study planner website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/my-study-planner.git
git push -u origin main
```

After each meaningful change, run:
```bash
git add .
git commit -m "Describe your actual change"
git push
```

## Jenkins integration
This simple project can use Jenkins to check out the GitHub repository and run a basic pipeline. Add a `Jenkinsfile` to the repository with stages for Checkout and checking that `index.html` exists. Configure a Jenkins Pipeline job to use **Pipeline script from SCM**, choose Git, enter your repository URL, select your branch, and set Script Path to `Jenkinsfile`. Then click **Build Now** and capture your own successful build screenshot.

## Evidence screenshots to add
Add your own screenshots to a folder named `evidence`:
- Website open in browser
- GitHub repository
- At least five real commits in Git history
- Jenkins pipeline and build result

Use clear filenames and add a short caption for each screenshot. Do not use fake screenshots or another student's work.

## Before submission
- Replace the GitHub URL placeholder with your real repository.
- Record your actual commit hashes.
- Add your own screenshots.
- Make sure the repository is accessible to your faculty.

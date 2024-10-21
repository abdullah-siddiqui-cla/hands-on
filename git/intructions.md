# Hands-on Git Session Manual
This document is designed for a hands-on session to practice using Git, a version control system. The focus is on how developers contribute to a shared repository collaboratively.

## Context
Imagine you're working at a company called [Intro-pal](https://github.com/abdullah-siddiqui-cla/git-intro), where every developer adds their introduction to the introduction.txt file in the repository. You notice that your name isn't included yet, so your task is to add it to the file to officially join the team.

## Task 1: Clone the Repository
- Open your terminal.
- Clone the repository using the command `git clone https://github.com/abdullah-siddiqui-cla/git-intro.git`
- Navigate to the folder (git-intro) that was created as a result of cloning the repository.

## Task 2: Create an Issue
In GitHub, create an issue to add your name into the `introduction.txt` file.

- Go to the "Issues" tab of the repository.
- Create a new issue with the title "[Your Name] - Add Introduction".
  - Add a brief description: "This issue is to add my introduction to the introduction.txt file."

## Task 3: Work on the Issue
Start working on the task of adding your name to the file.
- Fetch the dev branch from the origin (Hint: Use `git fetch` command)
- Checkout to `dev` branch (Hint: Use `git checkout` command)
- Create a new branch with name like `[your name]-add-introduction` (Hint: Use `git checkout -b [branch  name]`)
- Edit the introduction.txt file to add your name:

Format:

-- [Your Name] --

[An introductory line]

Example:

-- John Doe --

I enjoy coding and learning new technologies.

- Stage, commit and push the changes to the new branch. (Hint: Use `git add`, `git commit`, and `git push` command).

## Task 4: Create a Pull Request (PR)
Now that your changes are in GitHub, create a pull request (PR) to merge your branch into dev.

- Go to the "Pull Requests" tab in the GitHub repository.
- Click on "New Pull Request."
- Set the base branch to dev and compare it with your branch (<[your name]-add-introduction>).
- Add a descriptive title and summary, then submit the PR.

## Task 5: Review a Teammate’s Pull Request
You’ll now review a teammate’s PR to simulate peer review:

- Go to the "Pull Requests" tab and pick any of your team member’s PRs.
- Check the file changes.
- If you have any feedback, leave a comment. Otherwise, approve the PR by going to Review Changes > Approve.

## Task 6: Resolve Conflicts
If a conflict occurs when you attempt to merge your PR, resolve it:

- Git will notify you of the conflicts in the PR.
- Fetch the latest changes from dev. (Hint: Checkout to dev branch, pull the latest changes, checkout again to your branch, then do `git merge dev`, resolve the conflicts, commit the code, and push it to branch)

## Task 7: Merge dev into main
Once all PRs are merged into dev, it’s time to update the main branch:

- Checkout the main branch
- Merge dev into main

The main branch is now updated with the latest changes from dev and ready for deployment to the production environment.
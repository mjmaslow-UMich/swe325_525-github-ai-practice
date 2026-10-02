## AI interaction 1
Date: 10/01/2026
Assistant: Claude Sonnet 5.5
Purpose: Explain the difference between a repository, branch, commit, pull request, and issue.
Prompt or summary: Explain the difference between a repository, branch, commit, pull request, and issue.
Response: Task 1: Core GitHub concepts

Repository (repo): The project's home. It holds your files, the full history of changes, and the collaboration tools around them. Think of it as a project folder with a built-in time machine.

Branch: An independent line of development within a repo. The default branch is usually main. You create a branch (like feature/github-ai-workflow) to work on changes without touching the stable code. Branches are cheap, so you can have many at once.

Commit: A saved snapshot of your changes, with a message and an author. Commits make up a branch's history, and you can return to any one. A good commit is small and focused, with a message like "Add setup instructions to README."

Pull request (PR): A proposal to merge one branch into another, usually your feature branch into main. It shows the diff and gives teammates a place to review, comment, run automated checks, and approve before the merge happens.

Issue: A tracked item of work or discussion, such as a bug report, feature request, or question. Issues aren't tied to code changes. You can assign them, label them, and link them to PRs. Writing "Fixes #12" in a PR description closes issue #12 when the PR merges.

How they fit together: You file an issue describing a problem. You create a branch in your repository to fix it. You make one or more commits on that branch. You open a pull request to merge the branch back, which resolves the issue.


## AI interaction 2
Date:10/1/2026
Assistant: Claude Sonnet 5.5
Purpose: to teah me how to complete a pull request
Prompt or summary: can you provide me with a workflow on how to create a pull request?
Useful suggestion: # How to Create a Pull Request

## 1. Update your local main
```bash
git checkout main
git pull origin main
```
If you forked the repo, sync your fork on GitHub first.

## 2. Create a feature branch
```bash
git checkout -b feature/github-ai-workflow
```
Use a short, descriptive name that follows your course or team convention. Never work directly on `main`.

## 3. Make your changes
Edit the files you need (for example, `README.md`). Keep changes focused on one purpose.
```bash
git status
git diff
```

## 4. Stage and commit
```bash
git add README.md
git commit -m "Add setup instructions to README"
```
Write messages that say what changed and why. Several small commits are better than one huge one.

## 5. Push the branch to GitHub
```bash
git push -u origin feature/github-ai-workflow
```
The `-u` flag links your local branch to the remote one, so later pushes only need `git push`.

## 6. Open the pull request
1. On GitHub, click the **Compare & pull request** banner, or go to **Pull requests > New pull request**.
2. Set the **base** branch (usually `main`) and the **compare** branch (your feature branch).

## 7. Write a clear title and description
- Give a concise title.
- Explain what you changed, why, and how to verify it.
- Link related issues with `Fixes #12` so they close automatically on merge.
- If AI tools helped, note that here if your course requires it.
- Add reviewers and labels in the right sidebar.

## 8. Respond to review and merge
1. Make sure automated checks pass.
2. Address reviewer comments by committing to the same branch. The PR updates automatically.
3. Once approved, click **Merge pull request**, then delete the branch.
4. Sync locally:
```bash
git checkout main
git pull origin main
```
Decision: accepted / revised / rejected
Reason:
Related GitHub URL:

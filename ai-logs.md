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

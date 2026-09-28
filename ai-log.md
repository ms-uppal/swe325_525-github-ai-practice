Create or update ai-log.md with prompts, summaries, decisions, 
and links to the GitHub work.

6. Ask AI for GitHub assistance
Ask the AI assistant to help with at least three different GitHub-related tasks. You may use the following
categories:

## AI interaction 1
Date: 9/28
Assistant: Copilot
Purpose:
Prompt or summary:
Useful suggestion:
Decision: accepted / revised / rejected
Reason:
Related GitHub URL:
• Explain the difference between a repository, branch, commit, pull request, and issue.

I'll explain these core Git and GitHub concepts for you:
Repository
A repository (or "repo") is a project's complete version-controlled codebase. It contains all files, folders, and the entire history of changes. Think of it as a project directory that tracks every modification ever made to it.
Branch
A branch is a parallel line of development within a repository. The default branch is usually main or master. Branches allow multiple developers to work on different features simultaneously without interfering with each other. You can create a branch, make changes, and later merge it back into another branch (typically main).
Commit
A commit is a snapshot of your code at a specific point in time. Each commit includes:
•	The actual code changes (the "diff")
•	A commit message describing what changed and why
•	Author information and timestamp
•	A unique identifier (SHA hash) like bda6253dc3c7fc65be3e5f0d5eb5e374cf9e355c
Commits form a chain that creates your project's history.
Pull Request (PR)
A pull request is a proposal to merge changes from one branch into another (usually from a feature branch into main). It's the mechanism for:
•	Sharing code changes with your team
•	Getting feedback through code review
•	Discussing the changes in comments
•	Running automated tests before merging
•	Ensuring quality control before integration
Looking at your URL, you have a PR comparing main with the feature/github-ai-workflow branch.
Issue
An issue is a way to track work, bugs, feature requests, or discussions. Issues can be:
•	Bug reports
•	Feature requests
•	Tasks to be completed
•	Discussion topics
•	Project planning items
Issues can be linked to PRs and commits, creating a complete audit trail from the initial request through implementation and deployment.
________________________________________
In workflow: You create an issue to track needed work → you make a branch to work on it → you create commits as you make changes → you open a PR to propose merging your branch back to main → after review, the PR is merged → the repository now contains your changes.

## AI interaction 2
Date:
Assistant:
Purpose:
Prompt or summary:
Useful suggestion:
Decision: accepted / revised / rejected
Reason:
Related GitHub URL:
• Review your README.md for clarity and suggest revisions.
swe325_525-github-ai-practice
GitHub and AI Workflow Practice
This repository is used for SWE 325/525 lab practice. It documents the process of using GitHub features such as issues, branches, commits, pull requests, and code review, with support from AI tools to improve workflow and documentation.
The goal of this project is to practice common collaborative software development tasks in a real-world GitHub workflow, including:
•	creating and tracking issues
•	working on feature branches
•	making commits with clear messages
•	opening and reviewing pull requests
•	using AI assistance to improve technical communication and development tasks
Student: Munjaap Uppal
Course: SWE 325/525

## AI interaction 3
Date:
Assistant:
Purpose:
Prompt or summary:
Useful suggestion:
Decision: accepted / revised / rejected
Reason:
Related GitHub URL:
• Suggest a checklist for a complete pull-request description.
PR Description Checklist
1. Title
•	Clear, descriptive title (not generic like "Updates" or "Fixes")
•	Follows naming convention if your team has one (e.g., "feat:", "fix:", "docs:")
•	Summarizes the main change in 50 characters or less
2. Description Structure
What (Purpose)
•	Briefly explains what the PR changes and why
•	Links to related issue(s) using Closes #123, Fixes #456, or Relates to #789
•	Explains the problem being solved (if not obvious from the issue)
How (Implementation)
•	Describes the approach or solution at a high level
•	Mentions any trade-offs considered
•	Notes if this is a breaking change
•	References any relevant documentation or architectural decisions
Testing
•	Describes how the changes were tested
•	Lists any new test cases or test coverage added
•	Notes edge cases considered
•	Mentions any manual testing performed (if applicable)
Scope & Files
•	Notes areas affected (e.g., "Changes to auth module only")
•	Mentions if refactoring or cleanup was involved
•	Flags any dependencies or prerequisite PRs
3. Metadata & Labels
•	Assignee(s) set appropriately
•	Reviewer(s) requested (especially CODEOWNERS)
•	Relevant labels applied (e.g., bug, enhancement, documentation, breaking-change)
•	Milestone set (if applicable to release planning)
•	Project board linked (if applicable)
4. Checklist (Optional but Recommended)
•	Author-filled checklist confirming:
o	Code follows project style guide
o	Self-review completed
o	Comments added for complex logic
o	Documentation updated
o	No breaking changes (or documented)
o	All tests passing
o	No new warnings or linting issues
5. Screenshots/Evidence
•	Screenshots or GIFs for UI changes
•	Before/after performance metrics (if applicable)
•	Console output or logs for backend changes
•	Links to deployed preview (if applicable)
6. Deployment Notes
•	Migration steps required (if database/config changes)
•	Environment variables or secrets needed
•	Rollback plan (if high-risk)
•	Dependencies or version constraints
________________________________________
Template Example
Markdown
## What
Closes #42. This PR refactors the README.md to improve clarity and structure.

## Why
The current README has redundant sections and unclear purpose statements, making it harder for new contributors to understand the project scope.

## How
- Consolidated duplicate headings
- Clarified project purpose and learning objectives
- Reformatted student identification section
- Removed inline task comments

## Testing
Manual review of markdown rendering on GitHub.

## Scope
- `README.md` only — no code changes

## Checklist
- [x] Documentation updated
- [x] No breaking changes
- [x] Self-review completed

## AI interaction 4
Date:
Assistant:
Purpose:
Prompt or summary:
Useful suggestion:
Decision: accepted / revised / rejected
Reason:
Related GitHub URL:
• Explain what a GitHub history view shows.
What a GitHub History View Shows
1. Commits (The Core)
Each commit in the history represents a snapshot of your code at a specific point in time. The history displays:
•	Commit message — what changed and why
•	Author — who made the change
•	Date/time — when it was committed
•	Commit hash — unique identifier (e.g., e7a9ccb)
•	Parent commit — what came before (the chain of history)
2. Branch Context
•	Which branch the commits are on (e.g., feature/github-ai-workflow)
•	Branching points — where one line of development splits off from another
•	Merge commits — where branches rejoin the main timeline
3. Comparison View (Your PR URL)
When comparing two branches (like your main vs. feature/github-ai-workflow), the history shows:
•	All commits unique to the feature branch that aren't in main
•	Files changed between the two points
•	Specific diffs (additions, deletions, modifications) for each file
•	Who made each change — useful for understanding the evolution
4. Chronological Order
•	Most recent commits appear at the top
•	Older commits appear lower down
•	Forms a linear or branching timeline depending on your merge strategy
5. Related Information
•	Pull requests associated with commits (marked with PR numbers)
•	Issue references (if commits mention #123)
•	Tags or releases marking important versions
•	Contributor activity — who's been active and how frequently
________________________________________
In Your Repository
Your PR comparison view (main...feature/github-ai-workflow) specifically shows:
•	All new commits added in feature/github-ai-workflow
•	Every file modified between these two branches
•	The exact differences in each file
•	Who reviewed and approved (if merged via PR)
This helps you see exactly what your feature branch adds to the main codebase before merging, making it easy to assess scope, quality, and completeness.

## AI interaction 5
Date:
Assistant:
Purpose:
Prompt or summary:
Useful suggestion:
Decision: accepted / revised / rejected
Reason:
Related GitHub URL:
• Suggest clear commit messages for the three changes.
Here are clear, specific commit messages for each of the three changes in the branch:
•	docs: improve project README with purpose, scope, and student info
•	docs: add AI workflow log for prompts and decisions
•	docs: add workflow notes covering GitHub concepts and branch process
If you want them in a more GitHub-style conventional commit format, use:
•	docs: improve README purpose and student identification
•	docs: add AI workflow activity log
•	docs: add GitHub workflow notes for issues, branches, and PRs
These are better because they:
•	start with the type of change (docs)
•	clearly describe what changed
•	avoid vague wording like “update file” or “create or update”

## AI interaction 6
Date:
Assistant:
Purpose:
Prompt or summary:
Useful suggestion:
Decision: accepted / revised / rejected
Reason:
Related GitHub URL:
• Help turn your acceptance criteria into a pull-request checklist.
Based on the changes in your PR, here's a PR checklist that maps to your acceptance criteria:
Markdown
## Acceptance Criteria Checklist

### README.md Improvements
- [ ] README.md has been improved with clearer purpose and scope
- [ ] Removed duplicate "GitHub and AI Workflow Practice" heading
- [ ] Student identification is properly formatted: **Student:** Munjaap Uppal
- [ ] Project purpose clearly states this is for SWE 325/525 lab assignment
- [ ] (Optional) Added learning objectives or scope summary

### ai-log.md Created
- [ ] ai-log.md file has been created
- [ ] Contains section for AI prompts used during this work
- [ ] Contains section for decisions made
- [ ] Contains section for links to GitHub work (issues, PRs, commits)
- [ ] Includes summaries of AI-assisted tasks

### workflow-notes.md Created
- [ ] workflow-notes.md file has been created
- [ ] Explains GitHub issues and their purpose
- [ ] Explains branches (feature branches, main, etc.)
- [ ] Explains commits (snapshots, messages, history)
- [ ] Explains pull requests (review, merge, code quality)
- [ ] Mentions default branch or references feature/github-ai-workflow branch
- [ ] Written in clear, accessible language for lab participants

### General Quality
- [ ] All markdown files have proper formatting
- [ ] No broken links or references
- [ ] Content is clear and readable
- [ ] Files follow repository structure conventions
- [ ] Ready for merge to main
This checklist directly translates the task descriptions embedded in your files into verifiable acceptance criteria that reviewers can check before approving and merging your PR.

## AI interaction 7
Date:
Assistant:
Purpose:
Prompt or summary:
Useful suggestion:
Decision: accepted / revised / rejected
Reason:
Related GitHub URL:
• Identify assumptions or risks in your planned GitHub workflow.
Based on your repository configuration and planned workflow, here are the key assumptions and risks to be aware of:
Assumptions
1.	Merge strategy is flexible — Your repo allows all three merge types (merge commit, squash, rebase), so you can choose the clearest approach for the final PR.
2.	No branch protection rules — Both main and feature/github-ai-workflow are unprotected, meaning there are no mandatory code reviews, status checks, or approval requirements before merging.
3.	Single developer — The repo is new (3 days old) with you as the only contributor, so there's no coordination overhead or conflict risk.
4.	Direct merge possible — Since you have full admin permissions and no protections are enforced, you can merge directly without review if needed.
5.	Public visibility — The repository is public, so all commits, PRs, and history are visible to anyone.
________________________________________
Risks
Workflow/Process Risks
Risk	Impact	Mitigation
No code review step	Low quality control before merge; no second pair of eyes on changes	For a lab assignment, manually review your own changes before merging, or add a peer reviewer
No automated checks	Unable to catch lint errors, broken tests, or security issues automatically	Add GitHub Actions or CI/CD pipeline to run tests on PR creation
Incomplete task files	The ai-log.md and workflow-notes.md are stub files (just task descriptions, not actual content)	Complete these files with real prompts, decisions, and explanations before merging
Documentation completeness	README improvements haven't been actually implemented yet (still shows placeholder text)	Update README with clear purpose, scope, and learning objectives
Repository Health Risks
Risk	Impact	Mitigation
No branch protection	Accidental direct pushes to main could break the default branch	Enable branch protections: require PR reviews, run checks, and enforce clean history
Public repo without guidelines	Unclear contribution standards; hard to onboard future collaborators	Add CONTRIBUTING.md and issue/PR templates
No commit message standards	Inconsistent history makes it hard to understand why changes were made	Adopt conventional commits (feat:, fix:, docs:) and enforce via linting
Merge commit message not enforced	PR history could be unclear with generic merge messages	Configure merge commit title/message to PR_TITLE_AND_BODY for better tracking
Current PR Risks
Risk	Concern
Stub content in new files	ai-log.md and workflow-notes.md contain task descriptions, not actual content. Reviewers will flag these as incomplete.
README not truly improved	The README still has the placeholder task text at the end; the actual improvements haven't been implemented.
No clear acceptance criteria met	The PR files don't yet demonstrate understanding of the concepts they're supposed to document.
________________________________________
Recommended Actions Before Merging
1.	Complete the actual content:
o	Replace placeholder text in ai-log.md with real prompts and decisions
o	Write actual explanations in workflow-notes.md (not just task descriptions)
o	Update README with the improved structure suggested earlier
2.	Add branch protection (even for a lab):
o	Require at least 1 PR review
o	Dismiss stale reviews when new commits are pushed
o	Require status checks to pass (add linting, tests)
3.	Document your workflow:
o	Add a CONTRIBUTING.md with commit message guidelines
o	Create a PR template to ensure consistent descriptions
4.	Consider adding CI/CD:
o	GitHub Actions workflow to lint markdown
o	Automated checks to validate PR completeness
Would you like help implementing any of these safeguards?


At least one prompt must ask for an explanation, one must ask for a proposed improvement, and one must
ask for a review or checklist. You may accept, revise, or reject the suggestions; you remain responsible for the final repository content.





1. Which GitHub action or object was most useful to you, and why?
>>>Holistic Change Visibility The comparison shows all commits, files changed, and diffs between main and your feature/github-ai-workflow branch in one place. You didn't have to search through individual commit logs or file histories separately—everything is aggregated.

2. Which AI suggestion did you accept, and what made it useful?
>>>The Accepted Suggestion: PR Description Checklist (AI Interaction 3)
What it was: A structured 6-section template for writing complete pull request descriptions, including:

Title — clear, descriptive, following conventions
Description Structure — What/Why/How format
Testing — coverage and edge cases
Scope & Files — affected areas
Metadata & Labels — assignees, reviewers, labels
Deployment Notes — migrations, rollback plans

3. Which AI suggestion did you revise or reject, and why?
>>>1. AI Interaction 2: README Improvements — REJECTED (Implied)
What was suggested: The AI provided a comprehensive revised README with:

Clear project purpose and scope
Learning objectives listed
Better structure with sections
Professional description

4. What did you verify yourself instead of trusting the AI?
>>>The main branch (base) only has 2 commits: "Initial commit" and "Expand README with GitHub and AI workflow details"

5. What would you change in your GitHub workflow next time?
>>>Next time: Finish writing files before creating the branch. When you open a PR, reviewers should see complete, polished work—not stubs. The PR comparison view revealed this gap, but only because files weren't ready.

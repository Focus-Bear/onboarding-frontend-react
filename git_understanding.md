Why are PRs important in a team workflow?

  - PRs is important as it allows collaboration, code review and quality assurance before being merged into the main branch. Preventing breaking changes and encourage team discussion.

What makes a well-structured PR?

  - A clean and concise title. 
  - A concise but informative description.
  - Highlighted issues with context.
  - Small but focused changes.
  - Commit messages that are clear and informative.

What did you learn from reviewing an open-source PR?

  - Collaborators provide constructive feedback/opinions, request changes and approve once standards are met.

------------------------------------------

What makes a good commit message?

  - A good concise message is informative, concise, and written with imperative. Examples are "Add new feature" is good but "Added new feature" is bad.

  - It should explain what changed and why, not just a simple description and is followed by a short summary of informative but concise details.

How does a clear commit message help in team collaboration?

  - It helps the team quickly understand the purpose of each chang without reading the entire code.

  - Reviewers can immediately spot relevant updates to see and give feedback.

How can poor commit messages cause issues later?

  - Poor messages can be confusing and make it hard to track what was done. Can make developers/reviewers waste time trying to figure out which commit induced the problem.

  - It reduces accountability and slows the team for new contributors.

----------------------------------------

What does git bisect do?

  - It helps find the exact commit that introduced bugs. It uses Binary Search between a known good commit and a bad one. It automatically checks commits between until it finds the first bad commits.

When would you use it in a real-world debugging situation?

  - I would use this feature if a bug appears in between many iterations of commits, especially if I do not know what caused it.

How does it compare to manually reviewing commits?

  - Manually reviewing is slow and error-prone, especially large projects. git bisect is a far more effective and systematic automated process. it reduces the number of commits to tests form potentially hundreds down to a binary search.

----------------------------------------

What does each command do?

  - git checkout main: Restores a specific file fom the main branch without interacting with other changes.

  - git cherry-pick: Applies only a single commit from another branch to the current branch.

  - git log: Shows commit history, IDS, messages, authors and dates.

  - git blame: Displays who modified last on a line on each file together with dates.

When would you use it in a real project (hint: these are all really important in long running projects with multiple developers)?

  - Absolutely, together with multiple developers, I think this helps everyone stay on track on who is doing what with a full and concise information needed to avoid wasting time figuring out what changed and who did it.

What surprised you while testing these commands?

  - I think it surprises me that this, while it adds complexity to my understanding what it means to be a frontend developer, it does seem like this will be very helpful in the long run, especially if I internalize this later on.

----------------------------------------

What caused the conflict?

  - When I created a branch from a main file, I added both some texts from the same line and when I prompted, git put to my attention the merge conflict.

How did you resolve it?

  - I used VS code's merge editor to accept only the current change (I could have accepted both, or the incoming change.)  saved the file and committed.

What did you learn?

  - In a collaborative setting, I think merge conflicts are ultimately common, standard procedure. Having two branches modify the same part of a file tends to be, by how I see it, ubiquitous.

----------------------------------------

Why is pushing directly to main problematic?

  - I think, in my research, VS code sees it as untested changes. If anyone can just push, bugs can slip mid production and disrupt the project workflow of just trying to find and fix the issue.

How do branches help with reviewing code?

  - It acts as a sandbox coding area where you can test out code and correct it as you see fit before you can commit it to the main branch.

What happens if two people edit the same file on different branches?

  - I think it will detect as a merge conflict. The team must resolve it manually, deciding which direction to go.

----------------------------------------

What is the difference between staging and committing?

  - Staging selects which changes will be part of the commit. While commit records those staged changes is now permanently added to the repository history.

Why does Git separate these two steps?

  - I think it is more of freedom of control, you an stage and commit at will for any specified tasks that the development team needed instead of them trying to tip toe if both functions are one function instead.

When would you want to stage changes without committing?

  - It helps me select and prepare certain stages for commitment instead of dumping ALL chunks of code to every commit, causing mass confusion and delays.

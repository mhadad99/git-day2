Name : Mahammad Hassan Ahmed


delete local
1- git branch -d dev
2- git branch -d test

delete remote
1- git push origin :dev
- git push origin :test


1. Annotated Tags
Description: A full Git object stored in the repository as part of the history.
Contents:
Tagger’s name, email, and timestamp.
A message or description (useful for release notes or details about the tag).
Can optionally be signed and verified with GPG for security.
Use Case:
For releases or important milestones where you want to store additional metadata or sign the tag for authenticity.

2. Lightweight Tags
Description: A simple pointer to a specific commit, similar to a branch but immutable.
Contents:
Only the commit reference; no additional metadata.
Cannot be signed or include messages.
Use Case:
For temporary or quick references where metadata or signatures aren’t necessary.

When to use Rebase
To Update Your Branch

Rebase your branch onto the latest base branch (e.g., main) to include recent changes.


To Clean Up Commits

Use interactive rebase to squash or edit commits before merging.


To Avoid Merge Conflicts Later

Rebase frequently to resolve conflicts incrementally as the base branch updates.


How to list tags?
git tag


Delete Tags
●
To delete remote tag
git push origin --delete v1.0
●
To delete local tags
git tag -d v1.0
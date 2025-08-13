git log 
========
is a Git command that shows the commit history of your repository. By default, it lists commits starting from the most recent, along with details like commit hash, author, date, and commit message.

git log
=======
This will display something like
*******************************
commit 4e2f9c58f67a5e8c1b123456789abcdef123456
Author: John Doe <john@example.com>
Date:   Mon Aug 12 10:15:30 2025 +0530

    Fix bug in API response handling
--------------------------------------

# commands
----------
1. Basic Log
bash
Copy
git log
Shows full commit details (hash, author, date, message).

2. One-Line View
bash
Copy
git log --oneline
Short hash + commit message — great for quick overviews.

3. Graph + Branch Overview
bash
Copy
git log --oneline --graph --all --decorate
--graph → ASCII branch tree

--all → show all branches

--decorate → show branch & tag names

4. Show Last N Commits
bash
Copy
git log -n 5
Last 5 commits only.

5. Filter by Author
bash
Copy
git log --author="Alice"
Only commits by Alice.

6. Search in Commit Messages
bash
Copy
git log --grep="bug fix"
Find commits where the message contains "bug fix".

7. Show Changes in Each Commit
bash
Copy
git log -p
Includes the patch/diff for each commit.

8. Filter by Date
bash
Copy
git log --since="2025-08-01" --until="2025-08-10"
Commits in a date range.

9. Show Files Changed
bash
Copy
git log --name-only

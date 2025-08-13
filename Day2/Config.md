Git has 3 levels of configuration
Think of it like layers of rules. The closer the layer is to your current project, the stronger it overrides the others.


1️⃣ System Config — "House rules"

Applies to: Everyone on the computer, every repo.

Where stored: A Git config file inside the system’s Git installation folder.

Example use: If your company installs Git on all PCs and sets a common merge tool for everyone.

Command:

bash
Copy
Edit

git config --system --list



2️⃣ Global Config — "Your personal rules"
Applies to: All repos for your user account.

Where stored: In your home folder (~/.gitconfig or Windows user profile).

Example use: Your personal name, email, or default editor for commits.

Command:

bash
Copy
Edit
git config --global --list





3️⃣ Local Config — "This project’s rules"


Applies to: Only the current repo.

Where stored: Inside .git/config in that repo folder.

Example use: Using a different email just for this project.

Command:

bash
Copy
Edit

git config --local --list

## 2024-07-23 - `sed -i` creates backup files that must be deleted
**Learning:** Using `sed -i.bak` for in-place file edits is effective, but it leaves behind a backup file (e.g., `filename.bak`). Committing this file to version control is a critical error, as it bloats the repository and is considered bad practice. The code review correctly flagged this as a blocking issue.
**Action:** In the future, whenever I use a command that generates temporary or backup files (like `sed -i.bak`), I must add a cleanup step to my plan to delete these files before finalizing the submission.

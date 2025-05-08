📚 Git Branching & Merging for Freshers
Hello folks! 👋
If you're new to Git and want to learn how to create branches, add code, and merge changes back to the main project, you're in the right place.

Let’s break it down step by step — all from your Linux terminal 🐧.

✅ Step 1: Create a New Branch
bash
Copy code
git checkout -b feature-branch
📌 This command:

Creates a new branch called feature-branch

Switches you to it

You can name the branch anything — like add-footer, about-page, or fix-header.

✅ Step 2: Make Some Changes
Edit or create files using nano or any editor:

bash
Copy code
nano index.html
After editing:

Press Ctrl + X → Y → Enter to save and exit

✅ Step 3: Add & Commit Your Changes
bash
Copy code
git add index.html
git commit -m "Added footer section"
This saves your work in Git.

✅ Step 4: Push the New Branch to GitHub
bash
Copy code
git push -u origin feature-branch
Your branch is now on GitHub! 🚀

✅ Step 5: Merge Branch into main
Switch back to the main branch:

bash
Copy code
git checkout main
Merge your feature branch:

bash
Copy code
git merge feature-branch
✅ Step 6: Push the Merged Changes
bash
Copy code
git push origin main
Now your updates are live on GitHub in the main branch 🎉

✅ (Optional) Delete the Feature Branch
Once merged, you can safely delete the old branch:

bash
Copy code
git branch -d feature-branch
🧠 Quick Summary
Action	Command
Create branch	git checkout -b branch-name
Add changes	git add .
Commit	git commit -m "message"
Push branch	git push -u origin branch-name
Merge branch	git merge branch-name
Delete branch	git branch -d branch-name




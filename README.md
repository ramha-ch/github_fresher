# 🚀 Getting Started with Git and Linux – Step-by-Step Guide

**Hey folks!**  
Welcome to your **first step** into the world of Git and version control using Linux.  
You're doing great — just one step at a time, and you're already ahead! 💪

---

## ✅ Prerequisites

Update your package list:
```bash
sudo apt update
⚠️ Note: If you're logged in as root, you don't need sudo.

Install Git:

bash
sudo apt install git

✍️ Create a Sample File Using Nano
Create a file called index.html:

bash
nano index.html

Add some content inside:

html
<h1>This is the first line</h1>
<h2>This is the second line</h2>
To save and exit nano:

Press CTRL + X

Press Y to confirm saving

Press Enter

📁 Navigate to Your Project Directory
bash
cd /path/to/your/project

🚀 Initialize a Git Repository and Push to GitHub
Step-by-Step:
bash

git init
git add .
git commit -m "First commit"
git branch -M main
git remote add origin https://github.com/your-username/your-repo.git
git push -u origin main

⚠️ Troubleshooting: "Password Authentication Was Removed"
If you see this error:

vbnet
remote: Support for password authentication was removed on August 13, 2021.
Use a Personal Access Token (PAT) instead:

🔐 Generate a PAT:
Go to: https://github.com/settings/tokens

Click “Generate new token (classic)”

Select scopes like repo

Click Generate and copy the token

💡 Replace your remote URL (if needed):
bash
git remote set-url origin https://github.com/your-username/your-repo.git

🧠 When prompted during git push:
Username: your GitHub username

Password: your Personal Access Token

🛠️ Alternative Method: Use SSH (Recommended)
If you don’t want to use a token every time, SSH is a great one-time setup.

1. Generate an SSH key:
bash

ssh-keygen -t ed25519 -C "your-email@example.com"

Just press Enter to accept the default location.

2. Add your SSH key to GitHub:
bash

cat ~/.ssh/id_ed25519.pub

Copy the output, then:

Go to: https://github.com/settings/keys

Click "New SSH key"

Paste your key and give it a name (like “GitHub  Key”)

3. Switch Your Remote to SSH
bash

git remote set-url origin git@github.com:your-username/your-repo.git

Check it with:

bash

git remote -v

You should see:

origin  git@github.com:your-username/your-repo.git (fetch)
origin  git@github.com:your-username/your-repo.git (push)

4. Test SSH Connection
bash

ssh -T git@github.com

If successful:
Message shows as
Hi your-username! You've successfully authenticated………………………………….

✅ Push Your Code!
Final step:

bash

git push -u origin main
No username or password will be needed — Git will use your SSH key for authentication. 🎉

🙌 You're all set!
Thanks for following along! You’ve just learned how to:

Set up Git on Linux

Create and edit files

Push code to GitHub using both HTTPS and SSH

Keep going — this is just the beginning of your development journey! 🚀
![Uploading image.png…]()

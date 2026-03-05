# Git Lab 1

**Name:** Ahmed Mahmoud Amer

## Lab Steps

###1.Create SSH Key and connect to GitHub

ssh-keygen -t ed25519 -C "medoamer2189@gmail.com"
type %USERPROFILE%\.ssh\id_ed25519.pub
#Then add the public key to GitHub
#test ssh 
ssh -T git@github.com	

#2.Create Local Repository and link with Remote
mkdir git-lab1
cd git-lab1
git init
git remote add origin git@github.com:AhmedAmer10/git-lab1.git
git branch -M main
git push -u origin main

3.Create HTML file and make commits
notepad index.html  # Create the file and add HTML content
git add index.html
git commit -m "first commit"

# Add more paragraphs and make commits
git add index.html
git commit -m "second commit"
git add index.html
git commit -m "third commit"
git add index.html
git commit -m "fourth commit"

4.Delete last 2 commits
git reset --hard HEAD~2

5.Add new commit after deletion
notepad index.html  # Add a new paragraph
git add index.html
git commit -m "commit after deletion"

6.Amend last commit
notepad index.html  # Add "lab Done" at the end of the file
git add index.html
git commit --amend -m "finish"

7.Push changes
git push origin main --force

8.Revert last commit (Bonus)
git revert HEAD
git push origin main


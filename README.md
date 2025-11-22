

# Git & GitHub Compact Cheat Sheet

---

## 1️⃣ Config

- `git config --global user.name "Your Name"` → নাম সেট
- `git config --global user.email "you@example.com"` → ইমেইল সেট
- `git config --list` → কনফিগারেশন চেক

---

## 2️⃣ Repository

- `git init` → নতুন লোকাল repo
- `git clone <url>` → GitHub repo ক্লোন

---

## 3️⃣ Branch

- `git branch` → ব্রাঞ্চ লিস্ট
- `git branch <name>` → নতুন ব্রাঞ্চ তৈরি
- `git switch <name>` → ব্রাঞ্চ পরিবর্তন
- `git switch -c <name>` → নতুন ব্রাঞ্চ + switch
- `git merge <branch>` → অন্য ব্রাঞ্চ merge
- `git branch -d <name>` → লোকাল ব্রাঞ্চ ডিলিট
- `git push origin --delete <name>` → রিমোট ব্রাঞ্চ ডিলিট

---

## 4️⃣ Stage & Commit

- `git status` → পরিবর্তন চেক
- `git add <file>` → এক ফাইল stage
- `git add .` → সব পরিবর্তন stage
- `git commit -m "Message"` → commit
- `git commit -am "Message"` → modify + commit একসাথে

---

## 5️⃣ Remote (GitHub)

- `git remote -v` → রিমোট চেক
- `git remote add origin <url>` → সংযোগ
- `git push origin <branch>` → push
- `git pull origin <branch>` → pull
- `git fetch origin` → শুধু রিমোট ডেটা আনা

---

## 6️⃣ History & Diff

- `git log` → commit history
- `git log --oneline` → সংক্ষেপে
- `git log --graph --all` → গ্রাফিক্যাল হিস্ট্রি
- `git diff` → পরিবর্তন চেক
- `git show <commit_id>` → নির্দিষ্ট commit
- `git status -s` → সংক্ষিপ্ত status

---

## 7️⃣ Undo / Reset

- `git restore <file>` → unstaged undo
- `git restore --staged <file>` → staged undo
- `git reset --hard <commit>` → সব পরিবর্তন reset
- `git revert <commit_id>` → undo commit নতুন commit হিসেবে

---

## 8️⃣ Stash

- `git stash` → hide changes
- `git stash list` → stash list
- `git stash apply` → stash apply
- `git stash drop` → stash remove

---

## 9️⃣ Branch Workflow

```bash
git switch main
git pull origin main
git switch -c feature-branch
git add .
git commit -m "Feature added"
git push origin feature-branch
# এরপর GitHub এ pull request তৈরি
```

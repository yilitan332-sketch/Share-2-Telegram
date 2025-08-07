    ✅ Connect it to your GitHub repo
    ✅ Pull changes from a remote branch (like fix-first-time-share-link)
    ✅ Start working on that branch properly

✅ 1. Open Git Bash inside your project folder

Make sure you're in the correct folder:

```
cd /f/github/Share-2-Telegram-main
```

✅ 2. Add the GitHub repo as a remote (you already did this)

You only need to do this once per project:

```
git remote add origin https://github.com/yilitan332-sketch/Share-2-Telegram.git
```

You can check it's there:

```
git remote -v
```

✅ Good if it shows:

origin  https://github.com/yilitan332-sketch/Share-2-Telegram.git (fetch)
origin  https://github.com/yilitan332-sketch/Share-2-Telegram.git (push)

✅ 3. Fetch the latest code from GitHub

This downloads the branches:

```
git fetch origin
```

✅ After this, you’ll see messages like:

From https://github.com/yilitan332-sketch/Share-2-Telegram
 * [new branch]      fix-first-time-share-link -> origin/fix-first-time-share-link

✅ 4. Check out and track the branch you want to work on

To switch to the remote branch fix-first-time-share-link:

```
git checkout --track origin/fix-first-time-share-link
```

💡 This does 2 things at once:

    Creates a local branch fix-first-time-share-link

    Sets it to track the remote branch origin/fix-first-time-share-link

✅ Now your Git Bash prompt should show:

(fix-first-time-share-link)

✅ 5. Confirm it worked

Use:

```
git branch -vv
```

✅ You should see something like:

* fix-first-time-share-link abc1234 [origin/fix-first-time-share-link] Commit message...

This means you’re working on a local copy of the remote branch.
✅ 6. Now you can pull, push, and commit as usual

    Pull latest changes:

```
git pull
```

Add and commit your work:

```
git add .
git commit -m "Your message"
```

Push your changes back:

```
    git push
```

✅ Summary of all commands (just copy/paste)

```
cd /f/github/Share-2-Telegram-main
```

```
git remote add origin https://github.com/yilitan332-sketch/Share-2-Telegram.git
```
```
git fetch origin
```
```
git checkout --track origin/fix-first-time-share-link
```
```
git branch -vv   # optional: to confirm tracking
```

Let me know if you:

    Want to start a new branch

    Want to push to a different remote

    Are still unsure what branch you're on
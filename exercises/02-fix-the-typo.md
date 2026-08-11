# Task 2 — Fix the typo

**Goal:** the headline says "Welcom". Fix it — and watch your fix travel from your Mac to the live website.

## Do this

1. In the repo folder, start Claude:
   ```
   claude
   ```
   and ask it:
   > There's a typo in the headline of index.html — please fix it and show me the change.
2. Leave Claude (`/exit`) and see what changed, yourself:
   ```
   git status
   ```
   (index.html is listed as *modified* — git noticed.)
   ```
   git diff
   ```
   Red line = how it was, green line = how it is now. Press `q` to get back out.
3. Save the change into history — a **commit**:
   ```
   git add index.html
   git commit -m "Fix headline typo"
   ```
4. Send it to GitHub — a **push**:
   ```
   git push
   ```
5. Refresh your local tab — fixed. Wait a minute, then refresh the live page — fixed there too.

## You should see

Your spelling fix, live on the internet, put there by you.

## What just happened

A **commit** is a snapshot with your name, the date, and your message stamped on it — it now exists forever in the project's history. A **push** uploads your new commits to GitHub, and the live page rebuilds itself from whatever is on GitHub. That's the loop you'll use for everything, always: **edit → commit → push**.

# Task 3 — Join the team board

**Goal:** your own card on the noticeboard, added by you, using the full loop from Task 2 — this time on your own.

## Do this

1. Open `index.html` and find the comment that says **TASK 3** (ask Claude to take you there if you like).
2. Copy the existing card — everything from `<li class="card">` down to `</li>` — paste it below the comment, and make it yours: your first name, what you do, and a fun fact.
3. Check what git noticed: `git status`, then `git diff`.
4. Commit it:
   ```
   git add index.html
   git commit -m "Add my card to the team board"
   ```
5. Push it:
   ```
   git push
   ```
6. Refresh the live page — you're on the board.

## Extra credit — see your change the way the team sees it

On github.com, open the repo and click **Commits** (top of the file list). There's your commit, with your name on it. Click it — the green and red lines are exactly what you changed. This is how teammates review each other's work.

## What just happened

Every change in git is **attributed**: history records who changed what, when, and — thanks to your commit message — why. That's why teams trust it: nothing is anonymous and nothing is lost.

# Task 1 — Get the repo onto your Mac

**Goal:** your own copy of this project (a "clone") in your Projects folder, and the noticeboard open in your browser.

## Do this

1. Open Terminal and go to your Projects folder:
   ```
   cd ~/Projects
   ```
2. Clone the repo (make your personal copy of it):
   ```
   gh repo clone Right-Formula/rf-git-training
   ```
3. Move into it:
   ```
   cd rf-git-training
   ```
4. Open the page straight from your Mac:
   ```
   open index.html
   ```
   The Team Noticeboard opens in your browser. This is **your local copy**.
5. Now open the **live version** in another tab:
   https://right-formula.github.io/rf-git-training/
   Same page — this one is published from GitHub.

## You should see

The noticeboard in two browser tabs: one served from your Mac, one live on the internet. (Spot anything odd about the headline? That's Task 2.)

## What just happened

"Cloning" gave you a full personal copy of the project — every file *and* its entire history. There are now two copies that matter: **yours** (on your Mac) and **GitHub's** (the shared one the website is built from). Git's whole job is keeping copies like these in sync.

**From now on:** whenever you work in here, start Claude first — type `claude` in this folder and it will guide you.

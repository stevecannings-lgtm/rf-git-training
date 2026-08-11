# Task 4 — Make it yours (change the colours)

**Goal:** repaint the whole page with one tiny edit, then read back the story of everything you've done so far.

## Do this

1. At the very top of `index.html` there's a comment that says **TASK 4**, next to a line like:
   ```
   --accent: #2E5496;
   ```
2. Change the colour. Plain colour names work: try `tomato`, `mediumseagreen`, `rebeccapurple`, `goldenrod` — or ask Claude to suggest a hex code for any shade you can describe.
3. Save, then run the loop — this time see if you can do it without looking anything up:
   ```
   git add index.html
   git commit -m "Repaint the noticeboard"
   git push
   ```
4. Refresh the live page. New look, shipped by you.

## Now read your story

```
git log --oneline
```

That's the project's diary — newest at the top, and the recent entries are yours. Press `q` if it opens a scrolling view.

## What just happened

Small commits with clear messages turn a project into a readable story. Anyone (including you, six months from now) can trace exactly how the page came to look the way it does.

**One more thing:** tell Steve you've finished Task 4. He'll switch the repo into "grown-up mode" — after that, changes can't go straight in; they go through review first. That's Task 5, and it's how real projects work.

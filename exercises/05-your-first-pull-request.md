# Task 5 — Your first pull request

**Goal:** add the team's first decision record (the ADR file Steve sent you) the way real teams ship changes: on a **branch**, through a **pull request**, reviewed, then **merged**.

Direct changes to `main` are now locked — try to imagine a bouncer standing in front of the live site. From here on, work goes in through review.

## Do this

1. Make sure you're up to date:
   ```
   git pull
   ```
2. Create a branch — a safe side-copy where you can work without touching the live site:
   ```
   git checkout -b add-first-adr
   ```
3. Put the ADR file Steve sent you into the `doc/adr/` folder (drag it there in Finder, or ask Claude to do it).
4. Make the decision visible on the noticeboard: in `index.html`, find the **TASK 5** comment and replace the "None yet" line with:
   ```
   <li><a href="https://github.com/stevecannings-lgtm/rf-git-training/blob/main/doc/adr/ADR-001-record-decisions-as-adrs.md">ADR-001 — Record decisions as ADRs</a></li>
   ```
   (Ask Claude if the HTML feels fiddly — that's what it's there for.)
5. Commit and push the branch:
   ```
   git add .
   git commit -m "Add ADR-001 and list it on the noticeboard"
   git push -u origin add-first-adr
   ```
6. Open the pull request:
   ```
   gh pr create --title "Add ADR-001" --body "Our first decision record."
   ```
   (Or click the yellow **Compare & pull request** button that appears on github.com.)
7. Tell Steve — he'll review it, maybe leave a comment, and merge it.
8. Once merged, bring your copy up to date and see the result:
   ```
   git checkout main
   git pull
   ```
   Refresh the live page — the Decisions section now lists ADR-001.

## What just happened

You just did the complete professional workflow: **branch → change → pull request → review → merge**. Nothing reached the live site until a second pair of eyes approved it. This is exactly how software teams — including ours — ship every change, and you've now done it end to end.

🎓 That's the course. You know git.

# RF Git Training Ground

A safe, breakage-proof repo for learning what git actually is — by changing a real, live website.

**The live page:** https://right-formula.github.io/rf-git-training/
(It's built from `index.html` in this repo. Push a commit, wait a minute, refresh — your change is live.)

## The loop

Everything in git comes down to one loop:

1. **Edit** a file on your Mac
2. **Commit** — save a snapshot of your change, with your name and a short message
3. **Push** — send your commits to GitHub
4. Look at it — on the live page, or in the repo's **Commits** tab on github.com

## The five tasks

Work through these in order — each one is a small file in the [`exercises/`](exercises/) folder.

| # | Task | What you'll learn |
|---|------|-------------------|
| 1 | [Get the repo](exercises/01-get-the-repo.md) | What a "clone" is |
| 2 | [Fix the typo](exercises/02-fix-the-typo.md) | The edit → commit → push loop |
| 3 | [Join the team board](exercises/03-join-the-team-board.md) | Doing the loop on your own |
| 4 | [Change the colours](exercises/04-change-the-colours.md) | Reading your history |
| 5 | [Your first pull request](exercises/05-your-first-pull-request.md) | Branches, PRs and review — the real workflow |

## Ground rules

- **You cannot break anything here.** That's the entire point of this repo. Worst case, we roll back — git remembers everything.
- **Claude is your co-pilot.** Open Terminal, go to this folder, type `claude`, and ask it anything — it knows this is a training repo and will explain as it goes.
- Small commits with clear messages beat big mysterious ones. Say what you changed and why.

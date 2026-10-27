
# Git Workflow and Merge Conflict Resolution

## Project Overview

As part of my GitHub Profile README assignment, I developed a professional GitHub profile while applying version control practices, including repository management, descriptive commits, and merge conflict resolution.

Throughout the project, I used Git and Visual Studio Code to manage local changes and synchronize updates with a remote GitHub repository. Each commit documented a specific stage of development, creating a clear record of the project's progression.

## Merge Conflict Resolution

To demonstrate conflict resolution, I intentionally modified the same line in `README.md` independently in my local repository and on GitHub.

After committing the remote change, I created a separate local commit and attempted to push it to the `main` branch. Git rejected the push because the remote branch contained changes that were not present in my local repository.

I retrieved the remote changes using:

```bash
git pull --no-rebase origin main
```

Git identified conflicting modifications in `README.md` that required manual resolution. Using Visual Studio Code, I reviewed the current and incoming changes, selected the appropriate version, and verified that all conflict markers were removed.

I then staged, committed, and pushed the resolved file:

```bash
git add README.md
git commit -m "Resolve merge conflict in README"
git push origin main
```

The final push completed successfully, and the merge resolution was recorded in the repository's commit history.

## Key Takeaways

This exercise reinforced the importance of understanding how Git manages changes across local and remote repositories. It also demonstrated why reviewing conflicting modifications is necessary before integrating changes into a shared codebase.

From a cybersecurity perspective, maintaining a clear and traceable version history supports accountability, change management, and the integrity of project documentation.

The experience strengthened my understanding of collaborative development workflows and the importance of resolving conflicts carefully to preserve the intended content.
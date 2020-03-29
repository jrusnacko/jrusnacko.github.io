# Branching in Git


<br>
Create a new branch and switch to it:

```bash
git checkout -b newbranch
```

Track a local branch with a remote:

```bash
git push -u origin newbranch
```

After the work is done, merge a branch into master:

```bash
git checkout master
git merge newbranch
```

Delete local branch:

```bash
git branch -d newbranch
```

Delete remote branch:

```bash
git push origin --delete newbranch
```

After deleting the remote branch, run this on all other machines to update references to deleted branches:

```bash
git fetch --all --prune
```


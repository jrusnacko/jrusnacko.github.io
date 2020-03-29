# Using Git diff


Simply running

```bash
git diff
```

shows changes not currently staged for commit. To show the staged changes, do

```bash
git diff --cached
```

The overview of changes across the repo can be gained by

```bash
git diff --stat
```

To set up vimdiff with git, run

```bash
git config --global diff.tool vimdiff
git config --global merge.tool vimdiff
git config --global difftool.prompt false
```

Then, use

```bash
git difftool <filename>
```

to see changes to a specific file. To compare the changes for a file with the last commit, use

```bash
git difftool HEAD^ <filename>
```


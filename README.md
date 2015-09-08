# pretty-git-for-bash
Add a pretty git prompt and some git aliases to your bash.

## Installation
clone this repository to your home directory.
```shell
cd ~
git clone https://github.com/cdue/pretty-git-for-bash.git
```

Then edit your .bashrc and add the following line:
`source ~/pretty-git-for-bash/bash_pretty_git`

Then restart you session, or type the following command line:
`source ~/.bashrc`

And you're done...

## What you get?

* A nice colored git prompt looking like:
  `user@host short-current-path (git-branch symbols) >`
  where symbols are:
  - '¤': working on non clear directory (untracked files, etc.)
  - '>': local branch is ahead of remote by X commits
  - '<': local branch is behind of remote by X commits
  - '<>': local and remote branches have diverged

* git aliases:
  - 'git l' : decorated git log


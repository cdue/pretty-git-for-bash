# pretty-git-for-bash
Add a pretty git prompt and some git aliases to your bash.
It does mostly the same as git bash prompt (ie. [link](https://github.com/git/git/blob/master/contrib/completion/git-prompt.sh))

## Installation
clone this repository to your home directory.
```shell
cd ~
git clone https://github.com/cdue/pretty-git-for-bash.git
```

Then edit your .bashrc and add the following line:
`source ~/pretty-git-for-bash/bash_pretty_git`

Then restart your session, or type the following command line:
`source ~/.bashrc`

And you're done...

If you experience some enoying latency, you can activate the "fast mode" (obviously faster but only display current branch name in prompt...).
To do so, just add the following line in your .bashrc (before the line you added before):
`export PRETTY_GIT_FAST_MODE=1`

then restart your session again:
`source ~/.bashrc`

## What you get?

* A nice colored git prompt looking like:
  `user@host short-current-path (git-branch symbols) >`
  where symbols (only available if you're not running in fast mode) are:
  - '¤': working on non clear directory (untracked files, etc.)
  - '>': local branch is ahead of remote by X commits
  - '<': local branch is behind of remote by X commits
  - '<>': local and remote branches have diverged

* git aliases:
  - 'git l' : decorated git log


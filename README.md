git-freebase adds enthusiasm and a sense of flow to your commits.

### Installation

Put git-freebase anywhere in your $PATH and mark it executable.

### Dependencies (you probably already have these)

* bash
* tr

### Use

Apply to your entire repository with:

    git freebase HEAD

The script passes its first argument to git-filter-branch as [rev-list options](https://git-scm.com/docs/git-filter-branch#git-filter-branch-ltrev-listoptionsgt82308203).

Being able to specify which revisions to use conveniently or precisely is not really in the spirit of this application, so any subsequent arguments are ignored.

### Warning

git-freebase modifies history. It uses `git filter-branch` to capitalize and remove punctuation from your commit messages. This is not an easy thing to undo.

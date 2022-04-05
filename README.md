>Git Commands

## git stash apply
This command takes the top most stash in the stack and applies it to the repo. In our case it is stash@{0}

If you want to apply some other stash you can specify the stash id.

Here’s the example:

git stash apply stash@{1}

## git stash pop
This command is very similar to stash apply but it deletes the stash from the stack after it is applied.

## git stash apply and pop
git stash pop throws away the (topmost, by default) stash after applying it, whereas git stash apply leaves it in the stash list for possible later reuse (or you can then git stash drop it).

## git stash clear
This command deletes all the stashes made in the repo. It maybe impossible to revert.

## git stash drop
This command deletes the latest stash from the stack. But use it with caution, it maybe be difficult to revert.

You can also specify the stash id.

git stash drop stash@{1}

# Rewinding Time with Git
1. Using git developer tools fine grained token to update local and remote repo without password. Fine grained token as a personal token is the password for the repo.

2. You can undo a push to the repo if already push [by doing this](https://stackoverflow.com/questions/1270514/undoing-a-git-push) using the following code below:

```
git push -f origin last_known_good_commit:branch_name
```

3. You can delete a remote branch once pushed to the [repo](https://www.freecodecamp.org/news/git-delete-branch-how-to-remove-a-local-or-remote-branch) using the following command below:

```
git push remote_name -d remote_branch_name
```

4. You can undo the last commit using ```git reset --[HARD/SOFT] ^HEAD-REF``` with `REF` being the number you want to rest by. More details [here](https://sethrobertson.github.io/GitFixUm/fixup.html) and [here](https://www.gitkraken.com/learn/git/git-reset#git-reset-hard)

> NOTE: Hard reset is used to permanently discard the commit you want to reset so should be used with caution

# Git Commands


# remove cached file/directory 
```sh
$ git rm -r --cached <file/directory>
```

# submodules
```sh
# add submodule 
$ git submodule add <repo> <path>

# update submodules from remote
$ git submodule update --init # only for the first time 
$ git submodule update --remote # from second time

# cloen with submodules recursively 
$ git clone --recurse-submodules <repo>


# remove a submodule
# https://gist.github.com/myusuf3/7f645819ded92bda6677
$ git deinit <path_to_submodule>
$ git rm <submodule>
$ rm -rf .git/modules/<path_to_submodule>
$ git commmit -m 'remove <submodule>'
$ git push


# check status
$ git check 

# check diff 
$ git diff --cached --submodule


# push submodules 
$ git push --recurse-submodules
```

# branching 
```sh
$ git checkout -b <new branch>
$ git checkout <branch>
$ git merge <branch>
$ git branch -d <branch> # delete local
$ git push origin --delete <branch> # delete eremote
```


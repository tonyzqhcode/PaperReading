

# Learning material

[git/github guide by Karl Broman](https://kbroman.org/github_tutorial/) 
[Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)




https://stackoverflow.com/questions/292357/what-is-the-difference-between-git-pull-and-git-fetch

`git fetch` updates your remote-tracking branches under refs/remotes/<remote>/. This operation is safe to run at any time since it never changes any of your local branches under refs/heads.

`git pull` brings a local branch up-to-date with its remote version, while also updating your other remote-tracking branches.

From the Git documentation for git pull:

In its default mode, git pull is shorthand for git fetch followed by git merge FETCH_HEAD.

https://stackoverflow.com/questions/3620633/what-is-the-difference-between-pull-and-clone-in-git

https://stackoverflow.com/questions/572549/difference-between-git-add-a-and-git-add?rq=1


# reset branch
https://stackoverflow.com/questions/1125968/how-do-i-force-git-pull-to-overwrite-local-files?rq=1 


# git rebase/git merge/git pull request
https://www.atlassian.com/git/tutorials/merging-vs-rebasing

https://stackoverflow.com/questions/2452226/master-branch-and-origin-master-have-diverged-how-to-undiverge-branches
https://stackoverflow.com/questions/804115/when-do-you-use-git-rebase-instead-of-git-merge

# git tree?

# How to add multiple GitHub accounts on the same computer?

## Method one

Change the user name and user email for a local repository


```
$ git config user.name qzhang

$ git config user.email qzhang@gatech.edu


```

## Creating a file using BASH
There are many ways to create a file using BASH.

using touch touch newFile.txt only creates.
using echo echo > newFile.txt only creates.
using cat cat > newFile.txt creates and can start appending to file.
using vim vim newFile.txt creates and can start editing the file.

[How to create a new file with vim](https://www.cyberciti.biz/faq/vim-new-file-creation-command-on-linux-unix/)


https://stackoverflow.com/questions/5834014/lf-will-be-replaced-by-crlf-in-git-what-is-that-and-is-it-important

https://stackoverflow.com/questions/1967370/git-replacing-lf-with-crlf

https://stackoverflow.com/questions/14005854/what-to-do-with-branch-after-merge
https://stackabuse.com/git-merge-branch-into-master/

https://stackoverflow.com/questions/2003505/how-do-i-delete-a-git-branch-locally-and-remotely

https://stackoverflow.com/questions/5195859/how-do-you-push-a-tag-to-a-remote-repository-using-git

 tar -xzf assignment3.tar.gz





# Pull repository and GitHub will request auth

[Method one ref](https://stackoverflow.com/questions/3860112/multiple-github-accounts-on-the-same-computer)

## Method two

Set up SSH Keys

[Method two ref](https://docs.github.com/en/enterprise-cloud@latest/authentication/connecting-to-github-with-ssh/about-ssh) [ref](https://betterprogramming.pub/how-to-use-multiple-github-accounts-with-one-computer-c9ba3f851b75)


# How to set a local repo?

Initial a git on your computer.
Navigate to the folder where you want to have a local repo.

```

git init 

```

```
git clone  https://github.gatech.edu/qzhang/HelloWorld.git

```
https://www.atlassian.com/git/tutorials/syncing

```
git status
git add .

git commit -m 'aaa'

git push

```


Setup a url

```
$ git remote add origin https://github.gatech.edu/qzhang/HelloWorld.git

```

Clone files

```
git pull  https://github.gatech.edu/qzhang486/HelloWorld.git

```

git pull will not set up a destination
```

$ git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using


```


```

$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master


```



```

$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/tonyzqhcode/OMSCS.git'


```

https://stackoverflow.com/questions/4181861/message-src-refspec-master-does-not-match-any-when-pushing-commits-in-git


https://stackoverflow.com/questions/37937984/git-refusing-to-merge-unrelated-histories-on-rebase



https://stackoverflow.com/questions/23401652/fatal-the-current-branch-master-has-no-upstream-branch
https://stackoverflow.com/questions/17096311/why-do-i-need-to-explicitly-push-a-new-branch/17096880#17096880
https://docs.github.com/es/enterprise-cloud@latest/get-started/using-git/pushing-commits-to-a-remote-repository
https://stackoverflow.com/questions/18031946/what-does-set-upstream-do
https://stackoverflow.com/questions/37770467/why-do-i-have-to-git-push-set-upstream-origin-branch


https://stackoverflow.com/questions/10002239/difference-between-git-checkout-track-origin-branch-and-git-checkout-b-branch/10002469#10002469
https://stackoverflow.com/questions/42830557/git-remote-add-origin-vs-remote-set-url-origin


https://stackoverflow.com/questions/16230838/is-it-possible-to-pull-just-one-file-in-git


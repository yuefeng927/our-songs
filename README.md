# Our Songs
A repo is created for students to practice working with Git Remotes.

## recycle-bin folder
You can add/delete/revise any files to this folder. This is the playground for you to practice.

## Instructions for Assignment

1. Fork https://github.com/udmis/our-songs to your account.
2. Clone your forked repo, e.g, `git clone https://github.com/yourname/our-songs.git`
3. Go to your local folder "our-songs" and check your remote settings:
```
$ git remote -v
origin	https://github.com/harrywang/our-songs.git (fetch)
origin	https://github.com/harrywang/our-songs.git (push)
```
4. Add https://github.com/udmis/our-songs as your upstream remote:
```
$ git remote add upstream https://github.com/udmis/our-songs
$ git remote -v
origin	https://github.com/yourname/our-songs.git (fetch)
origin	https://github.com/yourname/our-songs.git (push)
upstream	https://github.com/udmis/our-songs (fetch)
upstream	https://github.com/udmis/our-songs (push)
```
5. Check your local branches
```
$ git branch
master
```
6. Create a new branch so that you can add your code to the repo:
```
$ git checkout -b harry-wang
Switched to a new branch 'harry-wang'
$ git branch
harry-wang
master
```
7. Now, create a folder with your full name (all lowercase, no spaces, use hyphen between your first and last name), e.g., harry-wang and create a html file to show the title, artist, and lyrics of a song of your choice. (see an example in my folder)
8. Commit the changes to the local branch:
```
$ git add *
$ git commit -am 'added a song'
[harry-wang 5534235] added a song
 3 files changed, 54 insertions(+), 2 deletions(-)
 rewrite README.md (100%)
 create mode 100644 harry-wang/img/sailing-to-philadelphia.jpg
 create mode 100644 harry-wang/sailing-to-philly.html
 ```
9. Push your branch to your forked repo:
```
$ git push origin harry-wang
```
10. Go to Github and issue a Pull Request (PR) so that the Admin of the "upstream" repo can review and merge your code:
<img width="1006" alt="screen shot 2017-09-11 at 9 05 02 pm" src="https://user-images.githubusercontent.com/595772/30303294-06373596-9735-11e7-8261-bedfcd9bba40.png">
<img width="1038" alt="screen shot 2017-09-11 at 9 05 41 pm" src="https://user-images.githubusercontent.com/595772/30303296-073c9b2a-9735-11e7-8f03-5c2b5a031834.png">
11. The Admin of upstream review your PR (add comments if necessary) and merge your PR:
<img width="797" alt="screen shot 2017-09-11 at 9 09 33 pm" src="https://user-images.githubusercontent.com/595772/30303360-8734f480-9735-11e7-9eba-35edc14fa4ae.png">
<img width="785" alt="screen shot 2017-09-11 at 9 09 54 pm" src="https://user-images.githubusercontent.com/595772/30303367-94951812-9735-11e7-8053-ca1e7fe47c15.png">

12. Once the change is merged by the upstream admin, you should switch back to the local master branch, pull the changes from the upstream repo and remove the branch:

```
$ git checkout master
$ git pull upstream master
$ git push origin master
$ git branch -D harry-wang
```

Congratulations, you just finished your first Github Workflow Exercise!

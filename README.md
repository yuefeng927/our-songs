# Our Songs
A repo is created for students to practice working with Git Remotes.

## Instructions

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
7.
In the local folder, create a folder with your full name (all lowercase, no spaces, use hyphen between your first and last name), e.g., harry-wang and create a html file to show the title, artist, and lyrics of a song of your choice. (see an example in my folder)

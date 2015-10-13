# The Process of getting started

Apply `cd` to appropriate directory.

```
LaptopNames-MBP:~ laptop-name$ cd /Users/laptop-name/GitHub/getting-started
```
Apply `pwd` and `ls` to show path and list files.

```
LaptopNames-MBP:getting-started laptop-name$ pwd ; ls
/Users/laptop-name/GitHub/getting-started
```
I think this is a good time to install/create two files `README.md` and `LICENSE.md`, or just `SAVE AS` from a stock file directory, into *the appropriate directory*. Otherwise, the output will look like the following because there are no files to `add . ` Note, I prefer `SSH` instead of the `HTML` link.

```
LaptopNames-MBP:getting-started laptop-name$ git init ; git add . ; git commit -m 'First commit' ; git remote add origin ; git@github.com:otherness-space/getting-started.git ; git remote -v ; git push origin master
Initialized empty Git repository in /Users/laptop-name/GitHub/getting-started/.git/
On branch master

Initial commit

<strong>nothing to commit</strong>
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=<push|fetch>]
                          set up remote as a mirror to push to or fetch from

bash: git@github.com:otherness-space/getting-started.git: No such file or directory
error: src refspec master does not match any.
error: failed to push some refs to 'origin'
```

```
LaptopNames-MBP:getting-started laptop-name$ git remote add origin git@github.com:otherness-space/getting-started.git ; git remote -v ; git push origin master
origin	git@github.com:otherness-space/getting-started.git (fetch)
origin	git@github.com:otherness-space/getting-started.git (push)
error: src refspec master does not match any.
error: failed to push some refs to 'git@github.com:otherness-space/getting-started.git'
```

```
LaptopNames-MBP:getting-started laptop-name$ git status
On branch master

Initial commit

nothing to commit (create/copy files and use "git add" to track)
```

## Use `ls` to confirm file list in directory

```
LaptopNames-MBP:getting-started laptop-name$ ls
LICENSE.md	README.md
```

## Then:

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'First commit' ; git remote add origin git@github.com:user-name/repo-name-data.git ; git remote -v ; git push origin master
```

### Note the `fatal` output where I should have left something out.

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'First commit' ; git remote add origin git@github.com:otherness-space/getting-started.git  ; git remote -v ; git push origin master
[master (root-commit) blah] First commit
 2 files changed, 342 insertions(+)
 create mode 100644 LICENSE.md
 create mode 100644 README.md
fatal: remote origin already exists.
origin	git@github.com:otherness-space/getting-started.git (fetch)
origin	git@github.com:otherness-space/getting-started.git (push)
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 6.89 KiB | 0 bytes/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
 * [new branch]      master -> master
```

Check `git status`:

```
LaptopNames-MBP:getting-started laptop-name$ git status
On branch master
nothing to commit, working directory clean
```

The `git status` is clean.

Adding updates to files or adding files or basically adding any changes to anything from directory contents to within any listed file. I use:

```
git add . ; git commit -m 'Commit narrative ... ' ; git push origin master
```
or

```
git add . ; git commit -m '' ; git push origin master
```

Moving right along... I create this file `PROCESS.md`

```
LaptopNames-MBP:getting-started laptop-name$ ls
LICENSE.md	PROCESS.md	README.md
```
Then I do the `git add . ; git commit` etc.
```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'GitHub flavored markdown example' ; git push origin master
[master blah] GitHub flavored markdown example
 2 files changed, 8 insertions(+)
 create mode 100644 PROCESS.md
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 479 bytes | 0 bytes/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

This is just another example of typical output.

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Syntax highlighting example' ; git push origin master
[master blah] Syntax highlighting example
 1 file changed, 9 insertions(+)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 501 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Tables ex.' ; git push origin master
[master blah] Tables ex.
 1 file changed, 36 insertions(+)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 916 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'More mark sideways like task lists and references' ; git push origin master
[master blah] More mark sideways like task lists and references
 1 file changed, 27 insertions(+)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 743 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

The following happened to because the GitHub flavored references did not work when I replaced the posted info with my own. I posted the original next to my edit and they both did not work...

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Compare worky, nyet working' ; git push origin master
[master blah] Compare worky, nyet working
 1 file changed, 9 insertions(+)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 512 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

Rest ...

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'reset because there is something else happening because both do not work' ; git push origin master
[master blah] reset because there is something else happening because both do not work
 1 file changed, 8 deletions(-)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 341 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

You have to remember to place the text of the message otherwise you get denied.

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m '' ; git push origin master
Aborting commit due to empty commit message.
Everything up-to-date
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Formatting, lists, links' ; git push origin master
[master blah] Formatting, lists, links
 1 file changed, 64 insertions(+)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 803 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

This is the beginning where I noticed that the copied markdown did not function as posted. Formatting syntax doesn't seem to work over or within other formatting syntax.

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Edit markdown for ** effect' ; git push origin master
[master blah] Edit markdown for ** effect
 1 file changed, 1 insertion(+), 1 deletion(-)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 327 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

So I tried variations of the theme of error.

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Playing with ** effect' ; git push origin master
[master blah] Playing with ** effect
 1 file changed, 1 insertion(+), 1 deletion(-)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 322 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

Tried some more variations.

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Replaced ** with *' ; git push origin master
[master blah] Replaced ** with *
 1 file changed, 1 insertion(+), 1 deletion(-)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 321 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

Reflectively, I should have just bunched all the variations together... Would have been faster and perhaps less frivolous.

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Single ticks and single or double astericks do not cooperate together as formatting Github flavored markdown' ; git push origin master
[master blah] Single ticks and single or double astericks do not cooperate together as formatting Github flavored markdown
 1 file changed, 1 insertion(+), 1 deletion(-)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 371 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

Considered that maybe double underscores would have an effect but no...

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Applied double underscores as a replacement for **' ; git push origin master
[master blah] Applied double underscores as a replacement for **
 1 file changed, 1 insertion(+), 1 deletion(-)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 340 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

Oi.

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'I am not finding that double syntax usage formatting markdown does not work well or at all' ; git push origin master
[master blah] I am not finding that double syntax usage formatting markdown does not work well or at all
 1 file changed, 1 insertion(+), 1 deletion(-)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 363 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

I like horizontal rules.

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Horizontal rule?' ; git push origin master
[master blah] Horizontal rule?
 1 file changed, 5 insertions(+)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 317 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

I wanted the outline on the `<code>` tag but maybe it is a premiere feature for nonfreebies?

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'Test <code>Code</code>' ; git push origin master
[master blah] Test <code>Code</code>
 1 file changed, 3 insertions(+)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 354 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

And I try...

```
LaptopNames-MBP:getting-started laptop-name$ git add . ; git commit -m 'More code play' ; git push origin master
[master blah] More code play
 1 file changed, 1 insertion(+), 1 deletion(-)
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 339 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:otherness-space/getting-started.git
   blah..blah  master -> master
```

```
LaptopNames-MBP:getting-started laptop-name$

LaptopNames-MBP:getting-started laptop-name$
```

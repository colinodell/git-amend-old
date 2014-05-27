git-amend-old
=============

Bash script to amend older commits with staged changes.

Think of it like `git commit --amend`, but for older commits.

Special thanks to [@VonC](https://github.com/VonC) for [this StackOverflow answer](http://stackoverflow.com/a/3940887/158766) which provided the basis for this script.

Usage:
------

Once the script is added to your path, you can run it like so:

`git amend-old <target-rev>`

Where `<target-rev>` is the commit hash you'd like to merge your staged changes into.

**Example:**

```
# Edit some existing file
vi existing-file.ext
# Stage the changes you just made
git add existing-file.ext
# Combine the staged changes with commit abcd123
git amend-old abcd123
```

Caution:
--------

I have not thoroughly tested this script, but so far it seems to work okay for my personal usage.  It's possible that bugs exist which may cause undesired changes to your Git history.  By using this script you agree to the included [LICENSE](LICENSE).  If you do encounter a bug, I'd appreciate if you'd create an issue or patch for it.


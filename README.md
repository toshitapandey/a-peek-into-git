# A Peek Into Git
Understanding Git! 

### Dealing with remote

#### List remote
```
git remote -v
```
#### Add remote
```
git remote add upstream https://github.com/whoever/whatever.git
```

### Open source contribution

#### Merge/Sync remote (original repo) master into your (forked repo) branch 
[Reference](https://stackoverflow.com/a/7244456/666299)
```
# Add the remote, call it "upstream":

git remote add upstream https://github.com/whoever/whatever.git

# Fetch all the branches of that remote into remote-tracking branches,
# such as upstream/master:

git fetch upstream

# Make sure that you're on your master branch:

git checkout master

# Rewrite your master branch so that any commits of yours that
# aren't already in upstream/master are replayed on top of that
# other branch:

git rebase upstream/master

git push -f origin master
```


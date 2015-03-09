# impl2 4 br1

git remote add -f base https://github.com/michaellif/base.git

git subtree add --prefix base/ base master

git subtree pull --prefix base/ base master --squash
git pull -X subtree=base base master

git subtree push --prefix base/ base master

if "Working tree has modifications.  Cannot add." run
git checkout master

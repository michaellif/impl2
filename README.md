# impl2

git remote add -f base https://github.com/michaellif/base.git

git subtree add --prefix base/ https://github.com/michaellif/base.git master
git subtree add --prefix base/ base master

git subtree pull --prefix base/ https://github.com/michaellif/base.git master --squash
git subtree pull --prefix base/ base master --squash

git subtree push --prefix base/ https://github.com/michaellif/base.git master

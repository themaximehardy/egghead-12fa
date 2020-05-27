# Use Git Flow as a Reliable Version Control Model

### [Egghead link](https://egghead.io/lessons/git-use-git-flow-as-a-reliable-version-control-model)

## Commands

```
git init
touch README.md
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:themaximehardy/egghead-12fa.git
git push -u origin master
git checkout -b develop
git push -u origin develop
git checkout -b feature/foo develop
vim foo.js
git add foo.js
git commit -m "New foo file"
git checkout -b feature/bar develop
vim bar.js
git commit -m "New bar file"
git add bar.js
git commit -m "New bar file"
git checkout develop
git merge feature/foo
git checkout develop
git push
git checkout feature/bar
git log
git rebase develop
git log
git checkout develop
git merge feature/bar
git push
git checkout -b release/1.0 develop
git push -u origin release/1.0
vim foo.js
git commit -am "Update foo file"
git push
git checkout develop
git merge release/1.0
git push
git checkout master
git merge release/1.0
git push
git tag v1.0.0
git push origin v1.0.0
git checkout -b hotfix/fix-foo master
vim foo.js
git commit -am "Single foo after all"
git checkout master
git merge hotfix/fix-foo
git push
git tag v1.0.1
git push origin v1.0.1
git checkout develop
git merge hotfix/fix-foo
git push
git branch -d feature/foo
git branch -d feature/bar
git branch -d hotfix/fix-foo
git branch
```

## Links

[Gitflow Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)


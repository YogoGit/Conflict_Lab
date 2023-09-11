Lab to show conflict resolution

To demonstrate, clone this repository, and then attempt to merge two
branches which have conflicting commits to the master branch

View the changes on the main branch
```sh
% git checkout main
% git log
```
Note the changes in the feature branch
```sh
% git checkout feature1
% git log
```

Merge the changes on feature1 onto the main branch and verify
```sh
% git checkout main
% git merge feature1
% cat file.txt
```

Note the changes in the second feature branch
```sh
% git checkout feature2
% git log
% cat file.txt
```

Merge the changes on feature2 onto the main branch
```sh
% git checkout main
% git merge feature2
```

Deal with conflicts
```
[ Edit and save file.txt after resolvng conflicts ]
% git add file.txt
% cat file.txt
% git commit --no-edit
% git log
```

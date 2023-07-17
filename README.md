1. Create new branch
   `git checkout -b "<name_of_branch>"`

2. change brach
   `git checkout  master`

```
{
    "git log
commit d0cc6a5515108dce31fc53bc8d8f2b5853ac9794 (HEAD -> feature1, origin/master, master)
Author: Adarsh <sec@gmail.com>
Date: Sun Jul 16 02:22:16 2023 +0530

test commit"

" git log
commit ca1d2258691cb96bc43485e282f171eed9e82b41 (HEAD -> master, origin/master)
Author: Adarsh <jha01adarsh@gmail.com>
Date: Sun Jul 16 02:34:14 2023 +0530

    master commit

commit d0cc6a5515108dce31fc53bc8d8f2b5853ac9794 (feature2, feature1)
Author: Adarsh <jha01adarsh@gmail.com>
Date: Sun Jul 16 02:22:16 2023 +0530

    test commit"
}
```

3. Merge feature2 branch to master branch
   -> got to master
   `git merge feature2`

4. To get all the commit from github
   `git pull origin master`
   -> It means pull all the latest change from master and add it to my commits.

5. add->commit->pull->push
   In case of merge conflict, resolve the conflict,
   add->comm->pull->push

6. `git branch` -> list of all branch, active branch have \* on it.

7. Scenario :
   -> There is a master branch, feature branch .
   -> developer 1 is working on feature branch, once he's done with all the code , he go to master branch and merge feature branch to master branch using `git merge feature`.
   -> Once he merge, he do git commit , then git push to master. Meanwhile 2-3 developer push there code to master and commit it.
   So, we are getting error while commiting.
   -> what we will do:
   a. merge
   b. pull (`git pull origin master`)
   c. `git push origin master`
   ->

->But problem here is, no one is reviewing our code we just push to master (i.e, prod) branch.

-> That's why we never do merge locally and push to master .
correct way to do it is 'Pull request'

Pull Request :
go to the brach where , you are working, after all code.
git add
git commit
git pull
git push origin <branch name>

8. Get code on local
   `git clone <git .git>`

9. contribute to other persone repo/open source:
   a. fork the code
   b. clone the forked repo
   c. make changes commit to forked repo.
   d. create a pull request to original owner of repo.
   d. wait for merge

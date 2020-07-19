# Pull Request Steps

1. Fork project
2. Git clone repo
3. CD inside the directory
4. `git remote add upstream git@github.com:<pull request user>/example.git`
5. Create a branch: `git checkout -b <feature-branch-name>`  (example: fix-readme)
6. Make the changes you would like to make and save the file.
7. `git add <file>`
8. `git commit -m "give it a description"`
9. `git push origin <feature-branch-name>` (example: fix-readme)
10. Click compare & pull request in the user's PR repo and give a description to the PR.
11. Wait for the PR to be approved.
12. If not approved and you are asked to implement a change, you will go back to your branch (example: fix-readme), make the requested changes, commit them to your branch in your local machine, and push them to your branch on Github. Then the maintainer of the repo will receive a new email, he will look at your changes and hopefully she/he will approve and merge the changes.
13. Once approved, the master branch on the upstream project changed, so because you don't have yours synched with upstream yet you'll need to 1. `git checkout master` 2.  `git pull upstream master` <---because of this now our readme in master is the official readme with our change, the change we contributed.
14. Since we are done, we can delete the used branch (fix-readme) with `git branch -D feature-branch-name` (example: fix-readme)
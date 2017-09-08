per Tyge's suggestion, sent to BN 8/10/17

Hi Ben, Tyge suggested I give a brown bag demo of git/GitHub. I’ve found that I explain the same stuff to each of my pair programming partners when we set up our project to pass each other our work. If you think it would be helpful I’d be happy to cover some git basics:

`git`
1) explaining how a local git repo adds to the text editor (comparing git commits to “changes in memory” and “saved changes” in the text editor)
2) show how `git log` displays the chronological history of commits (and suggesting a useful strategy for making commits regularly with each step of the development)
3) explain how “master” is just a branch (show making a branch, switching between them and deleting branch)
4) suggest each member of the pair works in their own subfolder (similar to a workflow using branches but avoiding all the branch merging madness)
5) Establishing remotes (origin and upstream) for using GitHub (show how to make remotes, change them and delete them)

`GitHub`
1) user profile page displaying GitHub contributions (swanky on the resume/CV!)
2) easiest to work on the GH page to fork and clone or create a GH repo to clone locally (but you can start out a local git repo and then push it to GH)
3) LambdaSchool project >>> “driver” forks (then clones locally and on GH invites partner to be a collaborator)
4) “navigator” forks from “driver” repo (then clones locally) - this relationship is remembered on GH for when the Nav wants to make a PR to the Driver.
5) now both driver and nav have local git repo with origin: pointing to their GH repos
6) “navigator” establishes an upstream: `git remote add upstream <driver's GH URL>`

Now nav can make a PR to get their stuff to driver
Driver merges PR (should just be stuff in Nav sub-dir) and closes PR
Driver has Navs work!

Driver pushes their work to GH
Nav uses `git pull upstream master` to get Driver’s work
Now Nav has Drivers work!

Driver and Nav collaborate and in the Sprint/Lab projects parent folder, compile the final project for submission
Driver submits PR to LambdaSchool
Driver can open PR at beginning of project and all commits sent from Nav to Driver in PR and all pushes Driver makes will be added to the PR to Lambda School.

:tada:

If it’s too much for now, maybe a simpler demo of just using git for local work and explaining the difference between git and GitHub?

Let me know what you think :slightly_smiling_face:

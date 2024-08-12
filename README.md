# AEP

AYOT Enhancement Proposals


## TODO: Read first

- [Conventions](/ayot/aep/issues)


## Code of Conduct


#### Bug Report

Every bug report should consist of:

- A short, inclusive and exclusive title.
- Short description of what happened
- Environment
- Step-by-step guide to reproducing it again
- *Optional* Any additional details which helps to better understanding the 
  problem.


#### Feature request

- A short, inclusive and exclusive title.
- User story
- BDD scenario
- Wireframe or GUI prototype
- *Optional* Any additional details.


#### Question

- A short, inclusive and exclusive title.
- Environment
- A cut and clean question detail.


### Pull Request & Rebase

All contributers of a repository should first add their `ssh-key` to their 
`settings->SSH/GPG Keys` and do this for contribution:

- Make a fork of that repository.
- Get clone of your forked repository.
```bash
git clone <forked-remote>
```

- Also add main repository to your git working copy remotes as `upstream`.
```bash
git remote add upstream <main-remote>
```

- Create a branch for each issue, feture, as follow:
  * `feature/foo`
  * `fix/loginwhenuserisinactive`
  * `try/withkernel6`

- Make your changes and commit the changeset. Then push changes to your 
  forked repository. 
- Every commit message chould contains issue numbers(s), i.e
  * `Fix: Prevent login when user is deactivated. closes #78.`
  * `Fix: Foo problem. closes #65 and also closes ayot/bar#29.`
  * `Feature: Create /tokens REST API. needs more tests #74`

- Make pull request from your local branch to original repository. 
- Pull request title should describe content of the changeset.

For update your repositories with upstream:

- Fetch all remote repositories.
```bash 
git fetch --all
```

- Then rebase the origin.
``` bash
git rebase -i upstream/master
```

- If there is any conflict, fix them.
- Then push them to your fork.
```bash 
git push origin master 
``` 

Use `--force` if you know what you are doing.

> **_NOTE_**:  Git's output messages is the most favourit cookbook for git. 
  read them carefully.

This is a template repo. All new repositories within DE Experience Engg. team should fork from this repo.
To create a new repository from this template, follow the process mentioned [here](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template#creating-a-repository-from-a-template) (_ensure to select the option "Incude all branches"_)

## Tasks after creating the new repo
Ensure that following settings are done after creating the new repo from the template. One can have additional settings as required on top of the ones listed below.

- [ ] Add `@CognizantCodeHub/de-expengg` team in the _Settings / Collaborators and teams_. Ensure the role selected is `Write`.
- [ ] Create a new branch protection rule within `Settings` (follow the steps mentioned [here](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/defining-the-mergeability-of-pull-requests/managing-a-branch-protection-rule#creating-a-branch-protection-rule)). The new branch protection rule must have the following settings configured
  - [ ] "Branch name pattern" should be `main`
  - [ ] Under "Protect matching branches", 
    - [ ] select _Require a pull request before merging_.
    - [ ] select _Require approvals_, ensure _the Required number of approvals before merging_ is either `1` or more
    - [ ] select _Dismiss stale pull request approvals when new commits are pushed_
    - [ ] select _Require review from Code Owners_
    - [ ] select _Allow specified actors to bypass required pull requests_ and add `@CognizantCodeHub/de-expengg-core-reviewers` team to the list of actors
    - [ ] select Restrict who can dismiss pull request reviews and add `@CognizantCodeHub/de-expengg-core-reviewers` team to the list of actors

## Branches

### `main`
This is a protected branch. All commits to this branch must happen as a result of a reviewed pull request.

### `develop`
This is the trunk where all development should happen.

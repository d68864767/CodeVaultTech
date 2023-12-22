# Contributing

First off, thank you for considering contributing to this project. It's people like you that make this project such a great tool.

## Where do I go from here?

If you've noticed a bug or have a feature request, make sure to check our [issues](https://github.com/yourusername/yourprojectname/issues) if there's something similar to what you've observed or want to suggest. If there isn't, feel free to open a new issue!

## Fork & create a branch

If this is something you think you can fix or implement, then fork the repository and create a branch with a descriptive name.

A good branch name would be (where issue #325 is the ticket you're working on):

```shell
git checkout -b feature/325_add_japanese_locale
```

## Implement your fix or feature

At this point, you're ready to make your changes! Feel free to ask for help; everyone is a beginner at first.

## Write a good commit message

A good commit message serves at least three important purposes:

- To speed up the reviewing process.
- To help us write a good release note.
- To help the future maintainers of the project, it could be you.

Here's a few rules to make sure you are writing good commit messages:

- The first line should be a descriptive sentence about what the commit is doing, and it should be capable of being included in the release note.
- The second line should be empty.
- The third line and beyond is a detailed description of what happened in the commit. This includes:
    - What was the motivation of the commit.
    - How does it do what it was supposed to do.
- If your commit is related to an issue, add this at the end of your commit message: `refs #325`. If you are fixing an issue, use `fixes #325`. This will make sure the corresponding issue is closed when the commit is merged into master.

## Make a Pull Request

At this point, you should switch back to your master branch and make sure it's up to date with the master branch of the upstream repository:

```shell
git remote add upstream git@github.com:original-owner-username/original-repository.git
git checkout master
git pull upstream master
```

Then update your feature branch from your local copy of master, and push it!

```shell
git checkout feature/325_add_japanese_locale
git rebase master
git push --set-upstream origin feature/325_add_japanese_locale
```

Finally, go to GitHub and [make a Pull Request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) :D

## Keeping your Pull Request updated

If a maintainer asks you to "rebase" your PR, they're saying that a lot of code has changed, and that you need to update your branch so it's easier to merge.

To learn more about rebasing in Git, there are a lot of [good](https://git-scm.com/book/en/v2/Git-Branching-Rebasing) [resources](https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase) but here's the suggested workflow:

```shell
git checkout feature/325_add_japanese_locale
git pull --rebase upstream master
git push --force-with-lease feature/325_add_japanese_locale
```

## Merging a PR (maintainers only)

A PR can only be merged into master by a maintainer if:

- It is passing CI.
- It has been approved by at least two maintainers. If it was a maintainer who opened the PR, only one extra approval is needed.
- It has no requested changes.
- It is up to date with current master.

Any maintainer is allowed to merge a PR if all of these conditions are met.

## Thank you!

Your contributions to [project name] are greatly appreciated. Every little bit helps, and credit will always be given.

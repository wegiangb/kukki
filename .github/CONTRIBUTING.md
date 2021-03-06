# Contributing

Thank you for considering to contribute! :speech_balloon:


## Bugs :bug:

1. Search the issue tracker for similar bug reports before submitting a new one.
2. Specify the version of the library where the bug occurred.
3. Specify your browser version and operating system (e.g. `Chrome 0.0.0.0 (64-bit), Windows 0 (64-bit)`).
4. Describe the problem in detail. Explain what happened, and what you expected would happen.


## Pull Request Process :sparkles:

When contributing to this repository, please first discuss the change you wish to make with the owners of this repository via the issue tracker.
A proposed change should be focused and concise. Do not include generated build files in your commits.

1. Create a feature branch.
2. Implement your patch or feature on that branch. Maintain the existing coding style.
3. Lint and test your changes.
3. Add unit tests for any new or changed functionality.
3. Navigate to your fork on Github, select your feature branch and create a new Pull Request.
4. Once your PR has been merged, you can safely remove your feature-branch.


### Development :wrench:

This project contains scripts that will help you during development. All scripts can be executed with `npm run [script]`.
The following table provides an overview of the most important scripts:

| Task  | Description                           |
|-------|---------------------------------------|
| lint  | Checks source files for syntax errors |
| build | Generates the final bundle            |
| test  | Runs unit tests                       |

__Note__: Setting `BABEL_ENV` to `production` enables source code transpilation and minification which considerably slows down the build process.


### Keeping Things Up-To-Date :hourglass:

Don't merge new changes from upstream into your feature branch.
Instead, use `rebase` to replay all of your commits on top of the latest code base:

```sh
git checkout master
git pull upstream master
git checkout my-feature
git rebase master
```

Git will guide you through the process of resolving conflicts.
This operation is similar to merging, except you're in fact rewriting your local history.
After rebasing, you'll need to use `git push --force my-feature`.

You can add more commits to your feature branch after you created the PR.
This means that you can change things later if necessary.

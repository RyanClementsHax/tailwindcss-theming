# Contributing

## Questions

If you have questions about implementation details, help or support, then please use our dedicated community forum at [GitHub Discussions](https://github.com/RyanClementsHax/tailwindcss-themer/discussions) **PLEASE NOTE:** If you choose to instead open an issue for your question, your issue will be immediately closed and redirected to the forum.

## Reporting Issues

If you have found what you think is a bug, please [file an issue](https://github.com/RyanClementsHax/tailwindcss-themer/issues/new/choose). **PLEASE NOTE:** Issues that are identified as implementation questions or non-issues will be immediately closed and redirected to [GitHub Discussions](https://github.com/RyanClementsHax/tailwindcss-themer/discussions)

## Suggesting new features

If you are here to suggest a feature, feel free to [start a discussion](https://github.com/RyanClementsHax/tailwindcss-themer/discussions). From there, we will discuss use-cases for the feature and then finally discuss how it could be implemented.

## Development

### Online one-click setup

The fastest way to work on the repository is by using [Stackblitz's Codeflow](https://stackblitz.com/codeflow)

1. Click the `Open in Codeflow` button on this repo's README (or go directly to [this link](https:///pr.new/RyanClementsHax/tailwindcss-themer))
2. Run the build using `yarn watch`
3. Implement your changes and tests to files in the `src/` directory and corresponding test files
4. Use the example repos to integration test changes
5. Document your changes in the appropriate doc page
6. Git stage your required changes and commit (see below commit guidelines)
7. Submit PR for review

### Manual setup

If you prefer to not use Stackblitz for faster development, you can still do this the old fashioned way.

1. Fork this repository
2. Install dependencies by running `yarn install`
   - We use [yarn](https://yarnpkg.com/) v7 for package management
3. Run the build using `yarn watch`
4. Implement your changes and tests to files in the `src/` directory and corresponding test files
5. Use the example repos to integration test changes
6. Document your changes in the appropriate doc page
7. Git stage your required changes and commit (see below commit guidelines)
8. Submit PR for review

### Running examples

All examples are located in the `examples` directory of this repo.

1. Make sure you run `yarn watch` in the root of `tailwindcss-themer` to build the plugin and watch for any changes
2. Make sure you've installed the dependencies by running `yarn install` in the repo's root directory
3. Run `yarn start` in the selected examples' directory
4. After making a change to the plugin, restart the example's server (i.e. rerun `yarn start`) so that it picks up the changes

## Commit message conventions

`tailwindcss-themer` is using [Angular Commit Message Conventions](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#-commit-message-format). Please consult the guide for details on these conventions. Your PR might not be accepted if it does not abide by these conventions.

We have very precise rules over how our git commit messages can be formatted. This leads to **more readable messages** that are easy to follow when looking through the **project history**. This also makes **releases automatable** since version bumping is automated from commit messages using [semantic-release](https://github.com/semantic-release/semantic-release).

## Pull requests

For pull requests to be merged, they need to meet the following criteria:

- The feature/bug has a corresponding issue or discussion to track it
- The feature/bug has been identified as desired
- Tests are added for any changes
- All tests pass
- The code is readable
  - i.e. Others unfamiliar with your code can easy deduce it's meaning and future maintenance/extensions on it is easy to perform
  - Your code may be amazing, but you likely won't be the one maintaining it in the future so this goes a LONG way to ensure the long term health of the project
  - This also makes the project easier and more welcoming to contribute from others/newcomers

Maintainers merge pull requests by squashing all commits and editing the commit message if necessary using the GitHub user interface.

Use an appropriate commit type. Be especially careful with breaking changes.
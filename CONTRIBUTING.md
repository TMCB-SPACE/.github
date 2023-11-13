# CONTRIBUTING

Contributions are always welcome, no matter how large or small. 

Some thoughts to help you contribute to this project

## Recommended Communication Style

1. Always leave screenshots for visuals changes
2. Always leave a detailed description in the Pull Request. Leave nothing ambiguous for the reviewer.
3. Always review your code first. Do this by leaving comments in your coding noting questions, or interesting things for the reviewer.
4. Always communicate. Whether it is in the issue or the pull request, keeping the lines of communication helps everyone around you.

## Setup (forks are preferred).

First of all, understand the basics of [setting up a fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo).

Then, clone the repo using the docs over at [cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository).

Most of our repositories will use one of [Node.js](https://nodejs.org/en), [Python](https://www.python.org), or [Go](https://golang.org) for development. Please ensure you have the correct version of the language installed.

Each programming language will have a package manager, we will be generally using the one that is most supported and deterministic. Here's an example using [npm](https://docs.npmjs.com/getting-started) for package management: 

```shell
# use either of ssh or gh cli to clone the repo 
git clone git@github.com:<your name>/next.tmcb.space.git
gh repo clone TMCB-SPACE/next.tmcb.space

# change directory into the repo and install dependencies the deterministic way
cd next.tmcb.space
npm ci

# start the local development server
npm run dev
```

## Testing

For running the test suite, use the following command. Since the tests run in watch mode by default, some users may encounter errors about too many files being open. In this case, it may be beneficial to [install watchman](https://facebook.github.io/watchman/docs/install.html).

```shell
# the tests will run in watch mode by default
npm test

# optionally, you can lint and format most projects
npm run lint
npm run format
```

## Pull Requests

### _We actively welcome your pull requests, however linking your work to an existing issue is preferred._

1. Fork the repo and create your branch from `beta` or DEFAULT branch if different.
2. Name your branch something that is descriptive to the work you are doing. i.e. `feat-adds-new-thing` or `fix-mobile-scroll`.
3. If you've added code that should be tested, add tests.
4. If you've changed APIs, update the documentation.
5. If you make visual changes, screenshots are welcome.
6. Ensure the test suite passes.
7. Make sure you address any lint warnings.
8. If you make the existing code better, please let us know in your PR description.
9. A PR description and title are required. The title is required to begin with: "feat:" or "fix:"
10. [Link to an issue](https://help.github.com/en/github/writing-on-github/autolinked-references-and-urls) in the project. Unsolicited code is welcomed, but an issue is required for announce your intentions. PR's without a linked issue will be marked invalid and closed.

### PR Validation

Examples for valid PR titles:

- `fix: Correct typo`
- `feat: Add support for Node 21`
- `refactor!: Drop support for Node 6`

_Note that since PR titles only have a single line, you have to use the ! syntax for breaking changes._

See [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) for more examples.

### Work in progress
GitHub has support for draft pull requests, which will disable the merge button until the PR is marked as ready for merge.

## Issues

If you plan to contribute a change based on an open issue, please assign yourself by commenting on the following word `.take`. Issues that are not assigned are assumed open, and to avoid conflicts, please assign yourself before beginning work on any issues.

## Funding

@TMCB-SPACE is looking into funding options, currently tackling GitHub Sponsors and Patreon, but we are open to other options. If you have any suggestions, please let us know.

## License

By contributing to the @TMCB-SPACE projects, you agree that your contributions will be licensed under its [MIT license](https://choosealicense.com/licenses/mit/).

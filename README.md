# go-lib-template

Template/Boilerplate/Blueprint for Go libraries.

## Installation

```sh
go install github.com/tmrts/boilr
boilr template download -f neighborly/go-lib-template go-lib
```

## Usage

```sh
boilr template use go-lib <target-dir>
```

## Features

- [Release Drafter](https://github.com/toolmantim/release-drafter) using GitHub Actions.
- Travis CI.
- Go Modules
- Test suite using [Ginkgo](https://github.com/onsi/ginkgo).
- Readme & License.
- [EditorConfig](https://editorconfig.org/).

## GitHub Labels

We use a template for GitHub Labels. We use labels to guide changelog
generation and better understanding what is changing in Pull Requests.

### Install the CLI

We use the [github-label-sync](https://github.com/Financial-Times/github-label-sync) node package to sync labels to a GitHub repository.

```sh
npm install -g github-label-sync
```

### GitHub Access Token

Obtain a [GitHub personal access token](https://help.github.com/en/articles/creating-a-personal-access-token-for-the-command-line).
This is necessary for `github-label-sync` to access our GitHub repositories.

### Sync

Execute the following command to sync the labels:

```
github-label-sync --labels https://gist.githubusercontent.com/josemarluedke/984cbae3435a18818a5ae5d8aa44ff60/raw/github-labels.json --access-token <YOUR_GITHUB_TOKEN> neighborly/<REPO_NAME>
```

## License

This project is licensed under the [MIT License](LICENSE.md).

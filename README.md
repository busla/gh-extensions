# gh-extensions

This repository contains custom extensions for the [GitHub CLI (gh)](https://github.com/cli/cli#installation) to simplify common PR tasks.

## Extensions

### 1. gh-prc (Pull Request Create)

- Automatically pushes your current branch to the default remote
- Uses the first commit message as the PR title
- Creates a PR against the default branch
- Copies the PR URL to your clipboard
- Opens the PR in your default web browser

#### Usage

```bash
gh prc
```

### 2. gh-pru (Pull Request URL)

- Outputs the URL of the current pull request

#### Usage

```bash
# echo the URL
gh pru

# copy the URL to your clipboard
gh pru | <wl-copy|pbcopy>
```

### 3. gh-prw (Pull Request Web)

- Opens the current pull request in your default web browser

#### Usage

```bash
gh prw
```

## Installation

1. Make sure you have the GitHub CLI installed. If not, follow the [official installation guide](https://github.com/cli/cli#installation).
2. Clone this repository
3. Install the extensions

```bash
# enter the extension and install
cd <extension>
gh extension install . # installs extensions from the current directory
gh extension remove <extension> # remove extension

# or all of them at once
for dir in */; do (cd "$dir" && gh extension install .); done
```

## Contributing

Feel free to open issues or submit pull requests if you have suggestions for improvements or new extensions.

## License

This project is open source and available under the [MIT License](LICENSE).

# gh-extensions

This repository contains custom extensions for the GitHub CLI (gh) to enhance your workflow.

## Extensions

### 1. gh-prc (Pull Request Create)

This extension simplifies the process of creating a pull request from your current branch.

#### Features:

- Automatically pushes your current branch to the default remote
- Uses the first commit message as the PR title
- Creates a PR against the default branch
- Copies the PR URL to your clipboard
- Opens the PR in your default web browser

#### Usage:

```
gh prc
```

### 2. gh-pru (Pull Request URL)

This extension quickly retrieves the URL of the current pull request.

#### Features:

- Outputs the URL of the current pull request

#### Usage:

gh pru

## Installation

1. Make sure you have the GitHub CLI installed. If not, follow the [official installation guide](https://github.com/cli/cli#installation).

2. Clone this repository
3. Add the extensions to your GitHub CLI:

```bash
   gh extension create gh-prc
   gh extension create gh-pru
```

4. Copy the content of each extension file into its respective newly created file.

5. Make the extension files executable:

```bash
   chmod +x gh-prc
   chmod +x gh-pru
```

## Usage

After installation, you can use these extensions as part of your gh commands:

- To create a pull request: `gh prc`
- Output the URL of the current pull request: `gh pru | <wl-copy|some-other-cb>`
  - copy it to your clipboard (e.g. `wl-copy`): `gh pru | wl-copy`

## Contributing

Feel free to open issues or submit pull requests if you have suggestions for improvements or new extensions.

## License

This project is open source and available under the [MIT License](LICENSE).

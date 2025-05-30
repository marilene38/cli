
Markdown
# GitHub CLI

`gh` is GitHub on the command line. It brings pull requests, issues, and other GitHub concepts to the terminal—right where you work with `git` and your code.

![Screenshot of gh pr status](https://user-images.githubusercontent.com/98482/84171218-327e7a80-aa40-11ea-8cd1-5177fc2d0e72.png)

GitHub CLI is supported for users on GitHub.com, GitHub Enterprise Cloud, and GitHub Enterprise Server 2.20+ with support for macOS, Windows, and Linux.

---

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [Support](#support)
- [Roadmap](#roadmap)
- [Comparison with hub](#comparison-with-hub)
- [License](#license)

---

## Features

- Create, view, and manage issues and pull requests from the terminal
- Easily check the status of your work across multiple repositories
- Seamless integration with GitHub Actions and Codespaces
- Cross-platform support: macOS, Windows, Linux
- Authentication with GitHub.com and GitHub Enterprise
- Scripting and automation via rich command outputs

---

## Installation

See below for platform-specific installation instructions. For more details and troubleshooting, visit the [manual](https://cli.github.com/manual/).

### macOS

`gh` is available via [Homebrew][], [MacPorts][], [Conda][], [Spack][], [Webi][], and as a downloadable binary including Mac OS installer `.pkg` from the [releases page][].

> **Note:** As of May 29th, Mac OS installer `.pkg` are unsigned. See [`cli/cli#9139`](https://github.com/cli/cli/issues/9139) for updates on signing.

#### Homebrew

```sh
brew install gh
# To upgrade:
brew upgrade gh
MacPorts
sh
sudo port install gh
# To upgrade:
sudo port selfupdate && sudo port upgrade gh
Other macOS options: See table in the full installation section.

Linux & BSD
Debian and RPM repositories
Community-maintained repositories in various distros
OS-agnostic package managers: Homebrew, Conda, Spack, Webi
Releases page for precompiled binaries
For instructions, see Linux & BSD installation.

Windows
Via WinGet, scoop, Chocolatey, Conda, Webi, or MSI installers from the releases page.

WinGet
PowerShell
winget install --id GitHub.cli
# To upgrade:
winget upgrade --id GitHub.cli
Note: The Windows installer modifies your PATH. Open a new terminal window for changes to take effect.

Codespaces
To add GitHub CLI to your codespace, add the following to your devcontainer file:

JSON
"features": {
  "ghcr.io/devcontainers/features/github-cli:1": {}
}
GitHub Actions
GitHub CLI comes pre-installed in all GitHub-Hosted Runners.

Other Platforms
Download packaged binaries from the releases page.

Verification of binaries
Since version 2.50.0, gh has been producing Build Provenance Attestation.
See the manual for verifying releases.

Build from Source
See how to build GitHub CLI from source.

Usage
See the manual for detailed command documentation.

Example: Create a pull request

sh
gh pr create --title "My PR" --body "This is my pull request"
Example: List issues assigned to you

sh
gh issue list --assignee @me
For more examples, visit the usage guide.

Documentation
For installation options see above, for usage instructions see the manual.

Contributing
We 💖 contributions! If anything feels off or if some functionality is missing, check out the contributing page.
There you'll find our contributing guidelines, code of conduct, and instructions for:

Reporting bugs and suggesting features
Building the tool locally
Submitting pull requests
Running and writing tests
If you're a GitHubber interested in shipping new commands for the CLI, see our internal contributions doc.

FAQ for Contributors
How do I run tests?
See docs/project-layout.md for details.

How do I report a security vulnerability?
Please see our SECURITY.md for details.

Support
For questions and community support, use GitHub Discussions.
For bug reports or feature requests, open an issue in this repository.
Roadmap
See projects for the latest roadmap and planned features.

Comparison with hub
For many years, hub was the unofficial GitHub CLI tool. gh is a new project that helps us explore what an official GitHub CLI tool can look like with a fundamentally different design.
See our detailed explanation for more information.

License
This project is licensed under the MIT License.

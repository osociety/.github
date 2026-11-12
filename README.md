# Open Society organization defaults

This repository holds the files GitHub applies to every public Open Society
repository, so the same guide does not have to be copied into each one. A
default is only used when the repository does not have its own version of that
file.

| Path | What it does |
| :--- | :--- |
| [`profile/README.md`](profile/README.md) | The landing page at [github.com/osociety](https://github.com/osociety), plus the policy documents it links. |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Default contributing guide: toolchain, the checks CI enforces, and pull request expectations. |
| [`SECURITY.md`](SECURITY.md) | Default security policy — shown on each repository's Security tab and beside the private reporting form. |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | Contributor Covenant 2.1, covering issues, discussions, and pull requests. |
| [`ISSUE_TEMPLATE/config.yml`](ISSUE_TEMPLATE/config.yml) | Contact links on the **New issue** screen for repositories with no templates of their own. |
| [`pull_request_template.md`](pull_request_template.md) | Default pull request body for repositories without their own. |

## Who picks these up

`vernet` has its own issue templates, so it keeps them and inherits everything
else. `network_tools` and `network_tools_flutter` have no templates, so the
issue-form links above are what their **New issue** screen shows.

## Editing

Whatever lands on `main` here is live for the whole organization immediately —
the profile page and every Security tab included. Open a pull request when a
change deserves a look first.

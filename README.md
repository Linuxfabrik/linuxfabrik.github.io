<h1 align="center">
  Linuxfabrik Open Source
</h1>
<p align="center">
  Landing page for <a href="https://linuxfabrik.github.io/">linuxfabrik.github.io</a>, the GitHub Pages root of the Linuxfabrik organization. Points visitors at the documentation site of every public Linuxfabrik project.
  <span>&#8226;</span>
  <b>made by <a href="https://linuxfabrik.ch/">Linuxfabrik</a></b>
</p>
<div align="center" markdown>

![License](https://img.shields.io/github/license/linuxfabrik/linuxfabrik.github.io)
[![GitHubSponsors](https://img.shields.io/github/sponsors/Linuxfabrik?label=GitHub%20Sponsors)](https://github.com/sponsors/Linuxfabrik)
[![PayPal](https://img.shields.io/badge/Donate-PayPal-ff6600)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=7AW3VVX62TR4A&source=url)

</div>

<br />

# linuxfabrik.github.io

GitHub serves `https://linuxfabrik.github.io/` from a repository named after the organization. Without that repository the root path returns 404, while the project sites below it work. This repository fills the root with a landing page that lists every public Linuxfabrik project and links to its documentation.

The site is built with [MkDocs](https://www.mkdocs.org/) and the [Material](https://squidfunk.github.io/mkdocs-material/) theme, matching the look of all other Linuxfabrik documentation sites. Every push to `main` rebuilds and redeploys it via GitHub Actions.


## Scope

One page, `docs/index.md`. Project documentation stays in the project repositories and is only linked from here. See [CONTRIBUTING.md](CONTRIBUTING.md) for what belongs on the page and how to add a project.


## Local Preview

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --require-hashes --requirement .github/docs/requirements.txt
ln --symbolic --force ../CHANGELOG.md docs/CHANGELOG.md
ln --symbolic --force ../CODE_OF_CONDUCT.md docs/CODE_OF_CONDUCT.md
ln --symbolic --force ../CONTRIBUTING.md docs/contributing.md
ln --symbolic --force ../SECURITY.md docs/security.md
mkdocs serve
```

The symlinks mirror what the deployment workflow does; they are ignored by git.


## License

Released into the public domain under the [Unlicense](LICENSE).

# THD-Spatial Repository Template

This repository is a template for projects under the `THD-Spatial` GitHub group. It provides a basic structure, documentation, and guidance to help you prepare repositories for internal collaboration and open-source release.

## What this template includes

- `README.md` (project overview and usage guidance)
- `CONTRIBUTING.md` (contribution workflow and expectations)
- `LICENSE` (required before making a repository public)
- `docs/` (documentation pages for naming conventions and open-source readiness)
- `mkdocs.yml` (MkDocs configuration for documentation site generation)

## Before making a repository public

Use the open-source readiness checklist before publishing a repository under `THD-Spatial`.

- **Checklist:** [Open Source Checklist](docs/open-source-checklist.md)

The checklist covers:

- essential repository files (license, README, contributing, code of conduct)
- Git LFS setup for large files
- optional but recommended files
- final review steps before publication

## Repository naming

All repositories under `THD-Spatial` should follow a consistent naming convention.

- **Guidelines:** [Repository Naming Guidelines](docs/repository-naming.md)

## Required files for public repositories

### License (required)

> [!IMPORTANT]
> A public repository must include a license. Without a license, others do not have clear legal permission to use, modify, or distribute the code.
>
> Repositories under `THD-Spatial` must include a `LICENSE` file before being made public.

Useful resource:

- [Choose a License](https://choosealicense.com/)

### README (required)

> [!IMPORTANT]
> Every repository must include a `README.md` file that explains the project purpose, setup, and usage.

At minimum, the README should include:

- project title and description
- purpose / scope
- installation and usage instructions
- contribution guidance (or link to `CONTRIBUTING.md`)

### CONTRIBUTING (recommended, required for community-facing repos)

> [!IMPORTANT]
> Add a `CONTRIBUTING.md` file to explain how contributors should report issues, propose changes, and submit pull requests.

### Code of Conduct (recommended, strongly encouraged for public repos)

> [!IMPORTANT]
> A `CODE_OF_CONDUCT.md` file helps set expectations for respectful collaboration and creates a welcoming project environment.

A common choice:

- [Contributor Covenant](https://www.contributor-covenant.org/)

## Git LFS for large files

> [!IMPORTANT]
> Use Git LFS for large files (especially datasets, binaries, media, and generated assets) to keep the Git repository manageable.

Basic setup:

```bash
git lfs install
git lfs track "*.psd"
```

Then commit `.gitattributes` and your files as usual.

> [!NOTE]
> If you publish releases and want Git LFS files included in release archives, enable:
>
> **Settings → Archives → Include Git LFS objects in archives**

![GitHub release archives setting](docs/assets/archives_setting_screenshot.png)

## Optional but useful files

Depending on the project, consider adding:

- `CHANGELOG.md` — track notable changes
- `CODEOWNERS` — define review ownership
- `.github/ISSUE_TEMPLATE/` — issue templates
- `.github/pull_request_template.md` — PR template
- `SECURITY.md` — vulnerability reporting policy
- `SUPPORT.md` — support and contact guidance

## Documentation (MkDocs)

This template uses [MkDocs](https://www.mkdocs.org/) with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme for project documentation.

Documentation source files are located in the `docs/` directory.

### Run documentation locally

Install dependencies:

```bash
pip install -r docs/requirements.txt
```

Start the local docs server:

```bash
mkdocs serve
```

Then open:

- `http://localhost:8000/`

## Optional: Host docs on Read the Docs

To host the MkDocs site on Read the Docs:

1. Create a Read the Docs account.
2. Connect the GitHub repository.
3. Configure the project to build the docs (MkDocs).
4. Add a `readthedocs.yml` file to the repository root if needed.

Refer to the Read the Docs documentation for the latest MkDocs setup instructions.

---

## Notes for maintainers

This template is intended to be practical and easy to adapt. Keep it lightweight, remove sections you do not need, and update links/paths if you rename files in `docs/`.

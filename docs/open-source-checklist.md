# Open Source Readiness Checklist

This checklist ensures your repository meets all requirements for open-sourcing under the **THD-Spatial** group. Complete all items before making your repository public.

---

## Essential Requirements

Make sure following essential requirements are met before making your repository public:

[License](#license) | [README](#readme) | [Contributing Guidelines](#contributing-guidelines) | [Code of Conduct](#code-of-conduct)
### License
- [ ] `LICENSE` file created in repository root
- [ ] Appropriate license chosen (see [choosealicense.com](https://choosealicense.com/))
- [ ] License text copied into `LICENSE` file
- [ ] License committed to repository

> **Note:** Without a license, you are **not allowed** to make your repository public under **THD-Spatial** group.

### README
- [ ] `README.md` file created in repository root

#### README Content
  - [ ] Project title and description included
  - [ ] Project purpose clearly explained
  - [ ] Key features listed
  - [ ] Installation instructions provided
  - [ ] Usage examples included
  - [ ] Contribution guidelines referenced
  - [ ] README formatted with proper markdown

### Contributing Guidelines
- [ ] `CONTRIBUTING.md` file created in repository root
- [ ] Issue reporting process documented
- [ ] Pull request submission process documented
- [ ] Coding standards and best practices outlined
- [ ] Guidelines for writing commit messages included
- [ ] CONTRIBUTING.md linked in README

### Code of Conduct
- [ ] `CODE_OF_CONDUCT.md` file created in repository root
- [ ] Code of conduct chosen (e.g., [Contributor Covenant](https://www.contributor-covenant.org/))
- [ ] Contact information for reporting issues included
- [ ] CODE_OF_CONDUCT.md linked in README or documentation

---

## Data Management

### Git LFS (Large File Storage)
- [ ] Git LFS installed on local machine
- [ ] Git LFS initialized in repository (`git lfs install`)
- [ ] Large file types tracked (e.g., `git lfs track "*.psd"`, data files, etc.)
- [ ] `.gitattributes` file committed to repository
- [ ] Large files added and committed properly
- [ ] Release strategy for LFS files documented (if applicable)

> **Note:** Files tracked by Git LFS are not included in release assets by default. Please ensure to enable `Include LFS files in release assets` option in your repository settings if you want to include LFS files in your releases.

---

## Optional but Recommended Files

### CHANGELOG
- [ ] `CHANGELOG.md` file created
- [ ] Version history documented
- [ ] Changes formatted following [Keep a Changelog](https://keepachangelog.com/) format

### Issue and PR Templates
- [ ] `.github/ISSUE_TEMPLATE/` directory created (if using issue templates)
- [ ] Issue template(s) created
- [ ] `.github/PULL_REQUEST_TEMPLATE.md` file created
- [ ] PR template includes checklist for contributors

### Code Owners
- [ ] `CODEOWNERS` file created in root or `.github/` directory
- [ ] Code owners assigned for different parts of the repository
- [ ] Teams or individuals properly specified

### Security Policy
- [ ] `SECURITY.md` file created
- [ ] Security vulnerability reporting process documented
- [ ] Contact information for security issues provided
- [ ] Supported versions documented

### Support Guidelines
- [ ] `SUPPORT.md` file created
- [ ] Support channels documented (e.g., email, discussions, issue tracker)
- [ ] Response time expectations set (if applicable)

---

## Quality Checks

### Documentation Quality
- [ ] All documentation reviewed for clarity
- [ ] Spelling and grammar checked
- [ ] Links tested and working
- [ ] Code examples tested and verified

### Repository Settings
- [ ] Repository description added on GitHub
- [ ] Topics/tags added for discoverability
- [ ] Repository visibility set to Public
- [ ] Default branch configured (typically `main`)
- [ ] Branch protection rules configured (if needed)

### Code Quality
- [ ] Code reviewed and cleaned up
- [ ] Sensitive information removed (API keys, passwords, credentials)
- [ ] `.gitignore` file properly configured
- [ ] Dependencies documented
- [ ] Build/test instructions included (if applicable)

---

## Final Steps

- [ ] All essential requirements completed
- [ ] Repository tested by cloning fresh copy
- [ ] All links and references verified
- [ ] Project builds/runs successfully from scratch
- [ ] Team members notified about repository availability

---

## Repository is Ready!

Once all required checkboxes are marked, your repository meets the THD-Spatial group standards and is ready to be open-sourced!

**Date Completed:** [DD.MM.YYYY]

**Reviewed By:** [Reviewer Name(s)]

---

## Need Help?

If you have questions about any items in this checklist, please refer to the [README.md](README.md) for detailed guidance or contact the THD-Spatial group administrators.

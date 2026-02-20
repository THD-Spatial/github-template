# GitHub-Template

This is a template repository for GitHub projects under `THD-Spatial` group. It includes a basic structure and some common files you must have in your repository.

## Open Source Readiness Checklist

Before making your repository public under THD-Spatial group, use the **[OPEN_SOURCE_CHECKLIST.md](OPEN_SOURCE_CHECKLIST.md)** to ensure all requirements are met. This checklist includes:
- Essential requirements (License, README, Contributing, Code of Conduct)
- Data management (Git LFS configuration)
- Optional but recommended files
- Quality checks and final review steps

Complete the checklist to confirm your repository is ready for open source release.

---

## License

> [!IMPORTANT]
> It is important to include a license in your repository to specify how others can use your code. Without a license, others may not have the legal right to use, modify, or distribute your code. Without a license you are not allowed to make your repository public under `THD-Spatial` group.
>
To add a license to your repository, follow these steps:

1. Create a `LICENSE` file in the root of your repository.
2. Choose a license that suits your project. You can use [Choose a License](https://choosealicense.com/) to help you decide.
3. Copy the text of the chosen license into the `LICENSE` file.
4. Commit the `LICENSE` file to your repository.

## Git LFS

> [!IMPORTANT]
> You must use Git LFS to manage the large file most likely data files in your repository. 

Git Large File Storage (LFS) is a Git extension that allows you to manage large files in your repository. To use Git LFS, follow these steps:
1. Install Git LFS on your machine. You can download it from [Git LFS](https://git-lfs.github.com/).
2. Initialize Git LFS in your repository by running the following command in your terminal:
   ```git lfs install```
3. Track the file types you want to manage with Git LFS. For example, to track all `.psd` files, run:
   ```git lfs track "*.psd"```
4. Add the tracked files to your repository and commit them as usual. Git LFS will handle the large files and store them separately from your Git repository.

> [!NOTE]
> Make sure to enable `Include LFS files in release assets` option in your repository settings if you want to include LFS files in your releases. By default, files tracked by Git LFS are not included in release assets.
> 
> Settings -> Archives section -> Include LFS files in release assets (checkbox)
> ![alt text](image.png)

## Contributing

> [!IMPORTANT]
> If you want to contribute to this repository, please follow the guidelines in the `CONTRIBUTING.md` file. This file should include information on how to submit issues, create pull requests, and any coding standards or best practices you want contributors to follow.
> To create a `CONTRIBUTING.md` file, follow these steps:
1. Create a `CONTRIBUTING.md` file in the root of your repository.
2. Write clear and concise guidelines for contributing to your project. This may include:
   - How to report issues
   - How to submit pull requests
   - Coding standards and best practices
   - Any other relevant information for contributors
3. Commit the `CONTRIBUTING.md` file to your repository.
4. Make sure to link to the `CONTRIBUTING.md` file in your repository's README or other relevant documentation to ensure that potential contributors can easily find it.

## Code of Conduct

> [!IMPORTANT]
> It is important to include a code of conduct in your repository to set expectations for behavior and create a welcoming and inclusive environment for all contributors. A code of conduct helps to establish guidelines for respectful communication and collaboration, and it can help to prevent harassment and other negative behaviors in your project.
>To add a code of conduct to your repository, follow these steps:
1. Create a `CODE_OF_CONDUCT.md` file in the root of your repository.
2. Choose a code of conduct that suits your project. You can use [Contributor Covenant](https://www.contributor-covenant.org/) as a template.
3. Copy the text of the chosen code of conduct into the `CODE_OF_CONDUCT.md` file.
4. Commit the `CODE_OF_CONDUCT.md` file to your repository.
5. Make sure to link to the `CODE_OF_CONDUCT.md` file in your repository's README or other relevant documentation to ensure that all contributors are aware of the code of conduct and can easily access it.

## README

> [!IMPORTANT]
> A README file is essential for any repository as it provides an overview of the project, its purpose, and how to use it. A well-written README can help others understand your project and encourage contributions. To create a README file, follow these steps:
1. Create a `README.md` file in the root of your repository.
2. Write a clear and concise description of your project, including its purpose, features, and any relevant information for users and contributors.
3. Include instructions on how to install, use, and contribute to your project. This may include:
   - Installation instructions
   - Usage examples
   - Contribution guidelines
   - Any other relevant information for users and contributors
4. Use markdown formatting to make your README visually appealing and easy to read.
5. Commit the `README.md` file to your repository.
6. Make sure to keep your README up to date as your project evolves and changes over time. Regularly review and update the README to ensure that it accurately reflects the current state of your project and provides relevant information for users and contributors.

## Additional Files

Depending on the nature of your project, you may want to include additional files such as:
- `CHANGELOG.md`: A file to document the changes and updates made to your project over time.
- `CODEOWNERS`: A file to specify the code owners for your repository, which can help to manage contributions and ensure that the right people are notified of changes.
- `ISSUE_TEMPLATE.md`: A file to provide a template for users to submit issues, which can help to ensure that issues are reported in a consistent and organized manner.
- `PULL_REQUEST_TEMPLATE.md`: A file to provide a template for users to submit pull requests, which can help to ensure that pull requests are submitted in a consistent and organized manner.
- `SECURITY.md`: A file to provide information on how to report security vulnerabilities in your project, which can help to ensure that security issues are addressed in a timely and responsible manner.
- `SUPPORT.md`: A file to provide information on how to get support for your project, which can help to ensure that users can easily find the help they need when using your project.

# Documentation

For documentation we use the [mkdocs](https://www.mkdocs.org/) static site generator with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme. You can find the documentation source files in the `docs/` directory of this repository. To build and serve the documentation locally, follow these steps:
1. Install the required dependencies by running:
   ```pip install -r docs/requirements.txt```
2. Build and serve the documentation locally by running:
   ```mkdocs serve```
3. Open your web browser and navigate to `http://   localhost:8000/` to view the documentation.

## Hosting MkDocs Documentation on Read the Docs
To host your MkDocs documentation on Read the Docs, follow these steps:
1. Create an account on [Read the Docs](https://readthedocs.org/) if you don't already have one.
2. Connect your GitHub repository to Read the Docs by following the instructions on the Read the Docs website.
3. Configure your Read the Docs project to use MkDocs as the documentation builder. You can do this by adding a `readthedocs.yml` file to the root of your repository with the following content:
   ```yaml
   version: 2
   build:
     image: latest
   sphinx:
     builder: mkdocs
   ```
4. Push your changes to your GitHub repository, and Read the Docs will automatically build and host your documentation. You can access your documentation at `https://your-project-name.readthedocs.io/`.
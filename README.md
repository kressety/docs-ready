# GitHub Action: Download and Extract MD Files

## Overview

This GitHub Action is designed to download a specified GitHub repository, extract all Markdown (.md) files from it, and package them into a downloadable artifact. The action is triggered manually and requires the user to input the repository name in the format `owner/repo`.

## Features

- **Manual Trigger**: The action is triggered manually from the GitHub Actions tab.
- **Repository Input**: Requires the user to input a valid GitHub repository name.
- **MD File Extraction**: Extracts all `.md` files from the specified repository and its subdirectories.
- **Artifact Generation**: Packages the extracted `.md` files into a zip artifact.
- **Handling File Conflicts**: Manages file conflicts by creating numbered backups of files with the same name.

## Usage

1. **Create a Workflow File**:
   - Navigate to your GitHub repository.
   - Create a new directory `.github/workflows` if it doesn't exist.
   - Inside `.github/workflows`, create a new YAML file (e.g., `download_and_extract_md.yml`).

2. **Add the Workflow YAML**:
   - Copy the provided workflow YAML content into your newly created file.

3. **Trigger the Workflow**:
   - Go to the Actions tab of your GitHub repository.
   - Find the workflow you just created and click on "Run workflow".
   - Input the GitHub repository name you wish to process in the format `owner/repo`.

4. **Download the Artifact**:
   - Once the workflow run is completed, navigate to the "Artifacts" section of the workflow run summary.
   - Download the artifact containing the extracted `.md` files.

## Contributing

Contributions to improve this GitHub Action are welcome. Feel free to fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). See the LICENSE file for details.
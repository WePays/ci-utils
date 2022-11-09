# CI Utils for WongNung
This repository is a collection of small(ish) utilities for the [WongNung/WongNung](https://github.com/WongNung/WongNung) repository.

All the tools are written based on GitHub-hosted runners. You can check their runner specification [here](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners#supported-runners-and-hardware-resources).

Most of the utilities run on `ubuntu-latest` image. Any other images might need modifications to utilities, feel free to fork and do that.

# Utilities
* [flake8-summarize](flake8-summarize): a utility made specifically for GitHub Actions Summary feature, in Actions you should redirect its output to `$GITHUB_STEP_SUMMARY`,
  Example:
  ```sh
  flake8-summarize >> $GITHUB_STEP_SUMMARY
  ```

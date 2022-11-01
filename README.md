# Microsoft Azure Documentation

Welcome to the open-source [documentation](/azure) of [Microsoft Azure](https://azure.microsoft.com). Please review this README file to understand how you can assist in contributing to the Microsoft Azure documentation.

## Getting Started

Contributing to open source is more than just providing updates, it's also about letting us know when there is an issue. Read our [Contributing guidance](CONTRIBUTING.md) to find out more.

### Prerequisites

You've decided to contribute, that's great! To contribute to the documentation, you need a few tools.

#### Github

Contributing to the documentation requires a GitHub account. If you don't have an account, follow the instructions for [GitHub account setup](https://learn.microsoft.com/contribute/get-started-setup-github) from our contributor guide.

#### Tools

To install necessary tools, follow the instructions for [Install content authoring tools](https://learn.microsoft.com/contribute/get-started-setup-tools) from our contributor guide.

## License

Please refer to [LICENSE](LICENSE), [LICENSE-CODE](LICENSE-CODE) and [ThirdPartyNotices](ThirdPartyNotices.md) for all Licensing information.

## Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information, see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

Starter Workflows

These are the workflow files for helping people get started with GitHub Actions. They're presented whenever you start to create a new GitHub Actions workflow.

If you want to get started with GitHub Actions, you can use these starter workflows by clicking the "Actions" tab in the repository where you want to create a workflow.



Directory structure

ci: solutions for Continuous Integration workflows
deployments: solutions for Deployment workflows
automation: solutions for automating workflows
code-scanning: solutions for Code Scanning
pages: solutions for Pages workflows
icons: svg icons for the relevant template
Each workflow must be written in YAML and have a .yml extension. They also need a corresponding .properties.json file that contains extra metadata about the workflow (this is displayed in the GitHub.com UI).

For example: ci/django.yml and ci/properties/django.properties.json.

Valid properties

name: the name shown in onboarding. This property is unique within the repository.
description: the description shown in onboarding
iconName: the icon name in the relevant folder, for example, django should have an icon icons/django.svg. Only SVG is supported at this time. Another option is to use octicon. The format to use an octicon is octicon <<icon name>>. Example: octicon person
creator: creator of the template shown in onboarding. All the workflow templates from an author will have the same creator field.
categories: the categories that it will be shown under. Choose at least one category from the list here. Further, choose the categories from the list of languages available here. When a user views the available templates, those templates that match the same language will feature more prominently.
Categories

continuous-integration
deployment
testing
code-quality
code-review
dependency-management
monitoring
Automation
utilities
Pages
Hugo
Variables

These variables can be placed in the starter workflow and will be substituted as detailed below:

$default-branch: will substitute the branch from the repository, for example main and master
$protected-branches: will substitute any protected branches from the repository
$cron-daily: will substitute a valid but random time within the day

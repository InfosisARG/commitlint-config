<!--


  ** DO NOT EDIT THIS FILE
  **
  ** 1) Make all changes to `provision/generator/README.yaml`
  ** 2) Run`task readme` to rebuild this file.
  **
  ** (We maintain HUNDREDS of open source projects. This is how we maintain our sanity.)
  **


  -->

[![Latest Release](https://img.shields.io/github/release/InfosisARG/commitlint-config?style=flat-square)](https://github.com/InfosisARG/commitlint-config/releases/latest) [![Lint](https://img.shields.io/github/workflow/status/InfosisARG/commitlint-config/lint-code)](https://github.com/InfosisARG/commitlint-config/actions?workflow=lint-code) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow)](https://conventionalcommits.org) [![KeepAChangelog](https://img.shields.io/badge/changelog-Keep%20a%20Changelog%20v1.0.0-orange)](https://keepachangelog.com) [![Terraform Version](https://img.shields.io/badge/terraform-1.x%20|%200.15%20|%200.14%20|%200.13%20|%200.12.20+-623CE4.svg?logo=terraform)](https://github.com/hashicorp/terraform/releases) [![AWS Provider Version](https://img.shields.io/badge/AWS-3%20and%202.0+-F8991D.svg?logo=terraform)](https://github.com/terraform-providers/terraform-provider-aws/releases)

# commitlint-config

![commitlint-config](docs/images/diagrams/architecture/main.png)

Commitlint configuration

## Installation

### [yarn](https://yarnpkg.com)

If you're using [yarn](https://yarnpkg.com)

```shell
  yarn add --dev husky @commitlint/cli @commitlint/config-conventional @infosisarg/commitlint-config
```

### [npm](https://www.npmjs.com)

If you're using [npm](https://www.npmjs.com)

```shell
  npm i --save-dev husky @commitlint/cli @commitlint/config-conventional @infosisarg/commitlint-config
```

## Usage

# How to use this project

Create file `.commitlintrc.json` with extending preset and define set of scopes:

```json
{
  "extends": ["@commitlint/config-conventional"],
  "rules": {
    "type-enum": [
      2,
      "always",
      [
        // as examples
        "app",
        "common"
      ]
    ]
  }
}
```

Add to `package.json` next section:

```json
{
  "husky": {
    "hooks": {
      "commit-msg": "commitlint -E HUSKY_GIT_PARAMS"
    }
  }
}
```

## Examples

<!-- Space: Projects -->
<!-- Parent: CommitlintConfig -->
<!-- Title: Examples CommitlintConfig -->

<!-- Label: Examples -->
<!-- Include: ./../disclaimer.md -->
<!-- Include: ac:toc -->

### common

## Help

**Got a question?**

File a GitHub [issue](https://github.com/infosisarg/commitlint-config/issues).

## Contributing

See [Contributing](./docs/contributing.md).

## Module Versioning

This Module follows the principles of [Semantic Versioning (SemVer)](https://semver.org/).

Using the given version number of `MAJOR.MINOR.PATCH`, we apply the following constructs:

1. Use the `MAJOR` version for incompatible changes.
1. Use the `MINOR` version when adding functionality in a backwards compatible manner.
1. Use the `PATCH` version when introducing backwards compatible bug fixes.

### Backwards compatibility in `0.0.z` and `0.y.z` version

- In the context of initial development, backwards compatibility in versions `0.0.z` is **not guaranteed** when `z` is increased. (Initial development)
- In the context of pre-release, backwards compatibility in versions `0.y.z` is **not guaranteed** when `y` is increased. (Pre-release)

## Copyright

Copyright © 2018-2022 [Infosis Global](https://infosisglobal.com)

## Trademarks

All other trademarks referenced herein are the property of their respective owners.

## License

The code and styles are licensed under the LGPL-3.0 license [See project license.](LICENSE).

## Don't forget to 🌟 Star 🌟 the repo if you like commitlint-config

[Your feedback is appreciated](https://github.com/infosisarg/commitlint-config/issues)

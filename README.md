# install-wp-cli-github-action

Install wp-cli in your GitHub workflow

<!-- How to generate this file
```shell
npx --yes github-action-readme-generator@v1.7.2
```
-->
<div align="center" width="100%">
<!-- start title -->

# <img src="doc/assets/branding.svg" width="60px" align="center" alt="branding<icon:terminal color:blue>" /> GitHub Action: Install WP-CLI

<!-- end title -->
<!-- start badges -->

<a href="https://github.com/holyhope/install-wp-cli-github-action/releases/latest"><img src="https://img.shields.io/github/v/release/holyhope/install-wp-cli-github-action?display_name=tag&sort=semver&logo=github&style=flat-square" alt="Release" /></a><a href="https://github.com/holyhope/install-wp-cli-github-action/releases/latest"><img src="https://img.shields.io/github/release-date/holyhope/install-wp-cli-github-action?display_name=tag&sort=semver&logo=github&style=flat-square" alt="Release" /></a><img src="https://img.shields.io/github/last-commit/holyhope/install-wp-cli-github-action?logo=github&style=flat-square" alt="Commit" /><a href="https://github.com/holyhope/install-wp-cli-github-action/issues"><img src="https://img.shields.io/github/issues/holyhope/install-wp-cli-github-action?logo=github&style=flat-square" alt="Open Issues" /></a><img src="https://img.shields.io/github/downloads/holyhope/install-wp-cli-github-action/total?logo=github&style=flat-square" alt="Downloads" />

<!-- end badges -->
</div>

<!-- start description -->

Install WP-CLI utility in your GitHub workflow.

<!-- end description -->

<!-- start contents -->

This action installs the [WordPress CLI](https://developer.wordpress.org/cli/) from [GitHub releases](https://github.com/wp-cli/wp-cli/releases). It ensures the integrity and authenticity of the binary by verifying the signature and the checksum.

<!-- end contents -->

## Usage

<!-- start usage -->

```yaml
- uses: holyhope/install-wp-cli-github-action@main
  with:
    # Description: [Version of WP-CLI](https://github.com/wp-cli/wp-cli/releases) to
    # install. Default: `latest` version
    #
    version: ""

    # Description: True to check the WP-CLI binary's integrity and authenticity. False
    # to skip the checks.
    #
    # Default: true
    verify: ""
```

<!-- end usage -->

## Inputs

<!-- start inputs -->

| **<b>Input</b>**            | **<b>Description</b>**                                                                                    | **<b>Default</b>** | **<b>Required</b>** |
| --------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------ | ------------------- |
| <b><code>version</code></b> | [Version of WP-CLI](https://github.com/wp-cli/wp-cli/releases) to install.<br />Default: `latest` version |                    | **false**           |
| <b><code>verify</code></b>  | True to check the WP-CLI binary's integrity and authenticity. False to skip the checks.                   | <code>true</code>  | **false**           |

<!-- end inputs -->
<!-- start outputs -->

| **<b>Output</b>**        | **<b>Description</b>**     |
| ------------------------ | -------------------------- |
| <b><code>path</code></b> | Path to the WP-CLI binary. |

<!-- end outputs -->

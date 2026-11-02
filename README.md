[![StepSecurity Maintained Action](https://raw.githubusercontent.com/step-security/maintained-actions-assets/main/assets/maintained-action-banner.png)](https://docs.stepsecurity.io/actions/stepsecurity-maintained-actions)



<!-- markdownlint-disable -->


<p align="right"><a href="https://github.com/step-security/github-action-major-release-tagger/releases/latest"><img src="https://img.shields.io/github/release/step-security/github-action-major-release-tagger.svg?style=for-the-badge" alt="Latest Release"/></a><a href="https://github.com/step-security/github-action-major-release-tagger/commits"><img src="https://img.shields.io/github/last-commit/step-security/github-action-major-release-tagger.svg?style=for-the-badge" alt="Last Updated"/></a><a

</p>

GitHub Action that automatically generates or updates `v<major-release>` tags every time a new release is published.




## Introduction

This GitHub Action automatically generates or updates `v<major-release>` tags every time a new release is published, making it effortless to keep track of your project's major versions.

Imagine your Git repository has the following tags:

```
1.0.0
1.1.0
2.0.0
2.0.1
2.1.0
3.0.0
```

By simply incorporating Major Release Tagger, your repo will be enriched with the corresponding v-tags:

```
1.0.0
1.1.0    v1
2.0.0
2.0.1    v2
2.1.0
3.0.0    v3
```

When you create a new release tagged `3.1.0`, the `v3` tag will automatically point to it:

```
1.0.0
1.1.0    v1
2.0.0
2.0.1    v2
2.1.0
3.0.0
3.1.0    v3
```

Stay organized and efficient with Major Release Tagger - the ultimate GitHub Action to streamline your versioning process.




## Usage

```yaml
  name: Major Release Tagger

  on:
    release:
      types:
        - published

  jobs:
    publish:
      runs-on: ubuntu-latest
      steps:
        - uses: step-security/github-action-major-release-tagger@v1
```












## Related Projects

Check out these related projects.

- [Manage Release Branches GitHub Action](https://github.com/step-security/github-action-release-branch-manager) - GitHub Action that creates release branches on new major version update.
- [Release Drafter GitHub Action](https://github.com/step-security/release-drafter) - Drafts your next release notes as pull requests are merged into your default branch.


## References

For additional context, refer to some of these links.

- [Release Drafter GitHub Action](https://github.com/step-security/release-drafter) - Drafts your next release notes as pull requests are merged into your default branch.
- [Release Branch Manager GitHub Action](https://github.com/step-security/github-action-release-branch-manager) - Automatically creates "Long Term Support (LTS)" release branches when new releases are published




## License

<a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=for-the-badge" alt="License"></a>

<details>
<summary>Preamble to the Apache License, Version 2.0</summary>
<br/>
<br/>

Complete license is available in the [`LICENSE`](LICENSE) file.

```text
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  https://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
```
</details>

## Trademarks

All other trademarks referenced herein are the property of their respective owners.


---
Copyright © 2017-2025 [Cloud Posse, LLC](https://cpco.io/copyright)
Copyright 2026 StepSecurity

<a href="https://cloudposse.com/readme/footer/link?utm_source=github&utm_medium=readme&utm_campaign=step-security/github-action-major-release-tagger&utm_content=readme_footer_link"><img alt="README footer" src="https://cloudposse.com/readme/footer/img"/></a>

<img alt="Beacon" width="0" src="https://ga-beacon.cloudposse.com/UA-76589703-4/step-security/github-action-major-release-tagger?pixel&cs=github&cm=readme&an=github-action-major-release-tagger"/>

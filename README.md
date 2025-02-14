# psma1_vs

This repository provides a robust, standardized framework that streamlines research projects and adheres to open science principles.
Everything is included, from reproducible Python environments to an automated website pipeline.
Join us in advancing open science, promoting transparency, and accelerating innovation by adopting this comprehensive toolkit.

## Usage

To explore or contribute to this project, you must clone the git repository (preferable using `ssh`).

### Information

We have initialized an [Obsidian](https://obsidian.md/) vault at the repository root that we use to write literature, notes, reports, etc. in markdown.
Once cloned, you can open this repository by opening the repository directory as a Vault.

### Communication

> No research should be done alone.

We use this repository's issues as our todo list.
Asynchronous conversations about any of the tasks should be included as issue comments.
Synchronous meetings happening in-person or virtually should have meeting minutes stored in the [appropriate directory](01-management/03-meetings).

## Deploying

We use [bump-my-version](https://github.com/callowayproject/bump-my-version) to release a new version.
This will create a git tag that is used by [poetry-dynamic-version](https://github.com/mtkennerly/poetry-dynamic-versioning) to generate version strings.

However, we are using [Calendar Versioning](https://calver.org/) which means we need to manually specify new versions.
For example, to bump the version to November 8, 2024, you would run the following command after activating the relevant conda environment.

```bash
bump-my-version bump --new-version 2024.11.8
```

After releasing a new version, you need to push and include all tags.

```bash
git push --follow-tags
```

## License

Code contained in this project is released under the [GPLv3 license][gplv3] as specified in `LICENSE.md`.
All other data, information, documentation, and associated content provided within this project are released under the [CC BY-ND 4.0 license][cc-by-nd-4.0] as specified in `LICENSE_INFO.md`.

### Permissive release

On **January 1, 2040**, the above [GPLv3][gplv3] and [CC BY-ND 4.0][cc-by-nd-4.0] licenses are voided and superseded by the immediately following paragraph.

> Code contained in this project is released under the [MIT license][mit] as specified in `LICENSE.md`.
> All other data, information, documentation, and associated content provided within this project are released under the [CC BY 4.0 license][cc-by-4.0] as specified in `LICENSE_INFO.md`.

A manual permissive release can be made by the maintainers whenever they see fit by updating the license files and updating this section.

[gplv3]: https://spdx.org/licenses/GPL-3.0-only.html
[cc-by-nd-4.0]: https://creativecommons.org/licenses/by-nd/4.0/
[mit]: https://spdx.org/licenses/MIT.html
[cc-by-4.0]: https://creativecommons.org/licenses/by/4.0/

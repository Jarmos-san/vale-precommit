# Vale Pre-Commit Hook

This is the [`pre-commit`][1] hook for linting prose content written in Markdown
and/or Plain Text files using [`vale`][2].

**DISCLAIMER**: This repository is no longer maintained since the official
repository now supports `pre-commit` hooks. Please use the official repository
no onwards instead of this repository!

## Usage Guide

Like any other `pre-commit` hooks, adding this specific hook is as easy as
configuring your project's `.pre-commit-config.yaml` file! Simply add the
following lines of code to the aforementioned file & run the
`pre-commit install --install-hooks` command.

```yaml
repos:
  - repo: https://github.com/Jarmos-san/vale-precommit
    rev: v0.1.0
    hooks:
      - id: vale-system
```

Once you've set it up, [`git` pre-commit hooks][3] will take care of the rest
for you when you attempt to commit some changes to version control. Besides,
ensure you also have `vale` instead without which the hook will fail to run as
expected.

## Licensing & Distribution Rights

The project is licensed under the terms & conditions (T&Cs) of the [MIT][4]
License. So, you're free to redistribute, modify, copy & use the project's
source code as you see it fit as per the T&Cs of the license. For more
information on the usage & distribution rights, feel free to read the
[LICENSE][5] document.

<!-- Reference Links -->

[1]: https://pre-commit.com
[2]: https://vale.sh
[3]: https://git-scm.com/docs/githooks#_pre_commit
[4]: https://en.wikipedia.org/wiki/MIT_License
[5]: ./LICENSE

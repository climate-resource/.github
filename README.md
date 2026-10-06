# .github

Organisation-wide defaults for Climate Resource repositories.

- `.github/ISSUE_TEMPLATE/`: issue forms for bugs, features, tasks and epics.
  Bugs and epics are added to the [Engineering project](https://github.com/orgs/climate-resource/projects/2).
- `.github/pull_request_template.md`: the default pull request description.
- `profile/README.md`: the public profile shown on [github.com/climate-resource](https://github.com/climate-resource).

A repository uses these only when it has no files of its own.
Any `.github/ISSUE_TEMPLATE/` folder in a repository replaces all of the issue forms here,
so delete a repository's copies to pick these up.

This repository is public, because GitHub only applies defaults from a public `.github` repository.
Keep internal detail out of it.

## Renovate

`renovate/base.json` is the shared Renovate preset.
A repository extends it with `"extends": ["local>climate-resource/.github//renovate/base"]`.
Every non-major update lands in one weekly pull request that merges once its checks pass,
and each major gets its own pull request.

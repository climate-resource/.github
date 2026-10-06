# Renovate

`base.json` is the shared Renovate preset.
A repository extends it with `"extends": ["local>climate-resource/.github//renovate/base"]`.
Every non-major update lands in one weekly pull request that merges once its checks pass,
and each major gets its own pull request.

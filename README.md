# .github

Organization-wide defaults for `fayd-sa`.

| Path | Applies to |
|---|---|
| `.github/ISSUE_TEMPLATE/` | Default issue forms for any repo without its own: a work item and a decision, with blank issues off |
| `.github/PULL_REQUEST_TEMPLATE.md` | Default PR template for any repo without its own |
| `.github/CODE_OF_CONDUCT.md` | Default code of conduct |
| `.github/workflows/` | Reusable workflows, called by reference |

A repo that ships its own template overrides the default, and a repo with anything in its own
`.github/ISSUE_TEMPLATE/`, a `config.yml` included, gets none of the forms here. The defaults here carry only what is true everywhere and contain nothing
venture-specific.

The work item form applies the label `intake` and the issue type `Task`; the decision form applies
the label `lane:decide` and no type. A label a form
names has to exist in the repo the issue is filed in, or the issue is filed without it.

**This repository is public** — GitHub requires it for default community health files to apply.
Keep it that way: nothing describing ventures, products, or internal structure belongs here.
The members-only organization profile lives in `.github-private`.

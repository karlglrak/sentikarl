# Contributing to Sentinel/Sentikarl

## Branching

Changes to this project should be made on a `feature` branch with an appropriate descriptor for your work (e.g. `feature/add-contributing-md`).

Once a feature branch is ready for review (or earlier!) a pull request should be raised targeting the `master` branch.

## Testing

The [CI pipeline](https://github.com/karlglrak/sentikarl/actions/workflows/ci.yml) runs unit, integration and regression tests against each commit on both `feature` branches and the `master` branch.

The [CodeQL pipeline](https://github.com/karlglrak/sentikarl/actions/workflows/codeql.yml) is mostly there for my entertainment/edification, but raises security alerts against the project [here](https://github.com/karlglrak/sentikarl/security/code-scanning). Due to the long-running time of this pipeline, it is only enabled for new commits on the `master` branch.

## Updating Python or Poetry Versions

Python or poetry version changes should be reflected in the following files:
- [pyproject.toml](./pyproject.toml)
- [poetry.lock](./poetry.lock)
- [ci.yml](./.github/workflows/ci.yml)
- [codeql.yml](./.github/workflows/codeql.yml)


## OZI Project

This organization is the official working group for the development of OZI pure python packaging tools for the Meson build system.

Currently this project is in a Pre-alpha state.

## Motivation

### Commandline Toolchain

* Supply-chain as sourcecode; all packaging-related metadata in the pyproject.toml.
  * [x] NO setup.cfg
  * [x] NO setup.py

### Continuous Integration and Deployment

* Dependencies for the packaging process should be managed like actual source dependencies.
* A publishing tool should provide templated workflows:
  * [x] checkpoint - run dist, test, and lint checks; procure signed test log artifacts
  * [x] release - build [sigstore](https://sigstore.dev/) signed wheel and source releases
  * [x] generate-provenance - [SLSA v1.0 - Level 3](https://slsa.dev/spec/v1.0/levels#build-l3) provenance
  * [x] publish - publish releases to [PyPI](https://pypi.org/); and mirror releases, signature bundles, and provenance in a tagged release

## Goals

### Commandline Toolchain

* 🚧 Initialize and output pure Python package sources.
* 🚧 Track skipped coverage and quality assurance checks.

### Continuous Integration and Deployment

* 🚧 Be as CI/CD-provisioner agnostic as possible - GitHub is the only one supported for the time being, GitLab is a Work in Progress.

## Repositories

[<img align="left" width="380" src="https://raw.githubusercontent.com/OZI-Project/.github/main/github-metrics-repo-ozi.svg">](https://github.com/OZI-Project/OZI)
[<img align="left" width="380" src="https://raw.githubusercontent.com/OZI-Project/.github/main/github-metrics-repo-blastpipe.svg">](https://github.com/OZI-Project/blastpipe)

[<img align="left" width="380" src="https://raw.githubusercontent.com/OZI-Project/.github/main/github-metrics-repo-OZIProject_dev.svg">](https://github.com/OZI-Project/OZIproject.dev)
[<img align="left" width="380" src="https://raw.githubusercontent.com/OZI-Project/.github/main/github-metrics-repo-docs.svg">](https://github.com/OZI-Project/docs)

[<img align="left" width="380" src="https://raw.githubusercontent.com/OZI-Project/.github/main/github-metrics-repo-checkpoint.svg">](https://github.com/OZI-Project/checkpoint)
[<img align="left" width="380" src="https://raw.githubusercontent.com/OZI-Project/.github/main/github-metrics-repo-release.svg">](https://github.com/OZI-Project/release)
[<img align="left" width="380" src="https://raw.githubusercontent.com/OZI-Project/.github/main/github-metrics-repo-publish.svg">](https://github.com/OZI-Project/publish)
![Issue Metrics](https://raw.githubusercontent.com/OZI-Project/.github/main/github-metrics-issue-followup.svg)

<br/><br/>

### GitLab Components (externally hosted)

* [pipeline](https://gitlab.com/ozi-project/pipeline) - checkpoint, release, and publish components; work in progress.

### Forks (GitHub repositories)

* [mesonpep517](https://github.com/OZI-Project/mesonpep517)
* [pyc_wheel](https://github.com/OZI-Project/pyc_wheel)
* [python-email-validator](https://github.com/OZI-Project/python-email-validator)

### Forks (externally hosted, archived, development continues on GitHub)

* [mesonpep517](https://gitlab.com/ozi-project/forks/mesonpep517)

## Similar Projects

### Packaging
![PyPI - Version](https://img.shields.io/pypi/v/flit?style=plastic&logo=pypi&label=Flit&link=https%3A%2F%2Fflit.pypa.io%2Fen%2Fstable%2F&link=https%3A%2F%2Fpypi.org%2Fproject%2Fflit%2F)
![PyPI - Version](https://img.shields.io/pypi/v/hatch?style=plastic&logo=pypi&label=Hatch&link=https%3A%2F%2Fhatch.pypa.io%2Flatest%2F&link=https%3A%2F%2Fpypi.org%2Fproject%2Fhatch%2F)


### Dependency Management

![PyPI - Version](https://img.shields.io/pypi/v/poetry?style=plastic&logo=poetry&label=Poetry&link=https%3A%2F%2Fpython-poetry.org%2F&link=https%3A%2F%2Fpypi.org%2Fproject%2Fpoetry%2F)
![PyPI - Version](https://img.shields.io/pypi/v/pdm?style=plastic&logo=pdm&label=PDM&link=https%3A%2F%2Fpdm-project.org%2Flatest%2F&link=https%3A%2F%2Fpypi.org%2Fproject%2Fpdm%2F)


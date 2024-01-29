## OZI Project

This organization is the official working group for the development of OZI pure python packaging tools for the Meson build system.

## Goals

### Commandline Toolchain

* 🚧 Initialize and output pure Python package sources.
* Supply-chain as sourcecode; all packaging-related metadata in the pyproject.toml.
  * [x] NO setup.cfg
  * [x] NO setup.py
* 🚧 Track skipped coverage and quality assurance checks.

### Continuous Integration and Deployment

* 🚧 Be as CI/CD-provisioner agnostic as possible - GitHub is the only one supported for the time being, GitLab is a Work in Progress.
* Provide templated workflows:
  * [x] checkpoint - run dist, test, and lint checks; procure signed test log artifacts
  * [x] release - build [sigstore](https://sigstore.dev/) signed wheel and source releases
  * [x] generate-provenance - [SLSA v1.0 - Level 3](https://slsa.dev/spec/v1.0/levels#build-l3) provenance
  * [x] publish - publish releases to [PyPI](https://pypi.org/); and mirror releases, signature bundles, and provenance in a tagged release

## Repositories

### Python Packages

* [OZI](https://github.com/OZI-Project/OZI) - The focus of this organization, pure Python packaging with Meson.
* [blastpipe](https://github.com/OZI-Project/blastpipe) - OZI's end-to-end test suite.

### Project Web Resources

* [oziproject.dev](https://github.com/OZI-Project/OZIproject.dev) - The project homepage source.
* [docs.oziproject.dev](https://github.com/OZI-Project/docs) - The project documentation source. 

### GitHub Actions
  
* [checkpoint](https://github.com/OZI-Project/checkpoint) - This actions runs OZI specified checks of dist, lint, and test environments.
* [release](https://github.com/OZI-Project/release) - This action checks semantic-release and creates wheels per OZI specified Python minor versions supported and a source distribution, all release artifacts are signed with sigstore.
* [publish](https://github.com/OZI-Project/publish) - This action publishes the wheels, source distributions, and signatures.

### GitLab Components (externally hosted)

* [pipeline](https://gitlab.com/ozi-project/pipeline) - checkpoint, release, and publish components; work in progress.

### Forks (GitHub repositories)

* [pyc_wheel](https://github.com/OZI-Project/pyc_wheel)
* [python-email-validator](https://github.com/OZI-Project/python-email-validator)

### Forks (externally hosted)

* [mesonpep517](https://gitlab.com/ozi-project/forks/mesonpep517)

## Similar Projects

* [Flit](https://github.com/pypa/flit)
* [Hatch](https://github.com/pypa/hatch)
* [meson-python](https://github.com/mesonbuild/meson-python)
* [Python Dependency Manager](https://github.com/pdm-project/pdm)

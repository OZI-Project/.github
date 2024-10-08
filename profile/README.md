## OZI Project

This is the development home for the OZI packaging tool and related utilities.
Currently this project is in Beta; for more information please visit the [homepage](https://oziproject.dev/).

## Comparison of Python Packaging Tools

| Project                                      | [![OZI Badge](https://raw.githubusercontent.com/OZI-Project/brand/main/images/ozi-badge.svg)](https://oziproject.dev/) | [![Static Badge](https://img.shields.io/badge/-Flit-grey?logo=pypi)](https://pypi.org/project/flit/) | [![Static Badge](https://img.shields.io/badge/-Hatch-grey?logo=pypi)](https://pypi.org/project/hatch/) | [![Static Badge](https://img.shields.io/badge/-Poetry-grey?logo=poetry)](https://pypi.org/project/poetry/)     | [![Static Badge](https://img.shields.io/badge/-PDM-grey?logo=pdm)](https://pypi.org/project/pdm/)         | [![Rye](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/mitsuhiko/rye/main/artwork/badge.json)](https://rye-up.com) | [![PyScaffold](https://img.shields.io/badge/-PyScaffold?style=social&logo=pyscaffold&logoColor=005CA0&label=PyScaffold)](https://pyscaffold.org/) |
|----------------------------------------------|------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| Status                                       | Beta                                                                                                                  | Mature[^1]                                                                                              | Production/Stable[^2]                                                                                     | Mature[^1]                                                                                                        | Production/Stable[^3]                                                                                        | Alpha[^1]                                                                                                                                    | Production/Stable                                                                                                                                 |
| PyPI Package                                 | ✅                                                                                                                      | ✅                                                                                                    | ✅                                                                                                      | ✅                                                                                                              | ✅                                                                                                         | ❌                                                                                                                                         | ✅                                                                                                                                                 |
| Meson Integration                            | ✅                                                                                                                      | ❌                                                                                                    | ❌                                                                                                      | ❌                                                                                                              | ❌                                                                                                         | ❌                                                                                                                                         | ❌                                                                                                                                                 |
| Fast Dependency Resolution w/ ``uv``         | ✅[^4]                                                                                                                      | ❌                                                                                                    | ❌                                                                                                      | ❌                                                                                                              | ❌                                                                                                         | ✅                                                                                                                                         | ❌                                                                                                                                                 |
| CI Templates                                 | ✅                                                                                                                      | ❌                                                                                                    | ✅                                                                                                      | ❌                                                                                                              | ❌                                                                                                         | ❌                                                                                                                                         | ✅                                                                                                                                                 |
| Cython & C Extensions without ``setup.py``   | ✅                                                                                                                      | ❌                                                                                                    | ❌                                                                                                      | ❌                                                                                                              | ❌                                                                                                         | ❌                                                                                                                                         | ❌                                                                                                                                                 |
| Repo Size                                    | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/OZI-Project/OZI?label=%20)[^5]             | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/pypa/flit?label=%20)  | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/pypa/hatch?label=%20)   | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/python-poetry/poetry?label=%20) | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/pdm-project/pdm?label=%20) | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/astral-sh/rye?label=%20)                                   | ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/pyscaffold/pyscaffold?label=%20)                                   |
| Python Implementation                        | ![PyPI - Implementation](https://img.shields.io/pypi/implementation/OZI?label=%20)                                     | ![PyPI - Implementation](https://img.shields.io/pypi/implementation/flit?label=%20)                  | ![PyPI - Implementation](https://img.shields.io/pypi/implementation/hatch?label=%20)                   | ![PyPI - Implementation](https://img.shields.io/pypi/implementation/poetry?label=%20)                          | ![PyPI - Implementation](https://img.shields.io/pypi/implementation/pdm?label=%20)                        | ![Static Badge](https://img.shields.io/badge/cpython%20%7C%20pypy---?color=blue)[^6]                                                         | ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PyScaffold?label=%20)                                                         |
| Python Versions                              | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/OZI?label=%20)                                         | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flit?label=%20)                      | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Hatch?label=%20)                       | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry?label=%20)                              | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PDM?label=%20)                            | ![Static Badge](https://img.shields.io/badge/3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12---?color=blue)[^7]                       | ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyscaffold?label=%20)                                                             |

This was current as of August 2024 feel free to email help@oziproject.dev if you see something wrong.
[^1]: Assumption based on years in use and semantic version.
[^2]: Based on hatchling metadata
[^3]: Based on pdm-backend metadata
[^4]: OZI still uses ``pipx`` to provision *application* virtual environments, packages without entrypoints and plugins are installed with ``uv`` falling back to ``pip`` and ``pip-compile``.
[^5]: OZI requires ozi-templates which includes ~800kB of templates.
[^6]: See info at https://rye-up.com/guide/toolchains/
[^7]: Rye uses Python builds from https://github.com/indygreg/python-build-standalone

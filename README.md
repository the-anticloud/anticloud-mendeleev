# MENDELEEV

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-chemical_manufacturing-lightgrey)

> Anticloud-hardened packaging of the upstream project `MENDELEEV` in category **CHEMICAL MANUFACTURING**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** CHEMICAL MANUFACTURING · **Upstream:** https://github.com/lmmentel/mendeleev · **Upstream pin:** `bd4716bff94c7acf22210d6ffb75dbd1fcc4f9bc` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

[![Documentation Status](https://readthedocs.org/projects/mendeleev/badge/)](https://mendeleev.readthedocs.org)
[![Latest version released on PyPI](https://img.shields.io/pypi/v/mendeleev.svg?style=flat-square&label=PyPI%20version)](https://pypi.python.org/pypi/mendeleev)
[![MIT license](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![image](https://anaconda.org/conda-forge/mendeleev/badges/version.svg)](https://anaconda.org/conda-forge/mendeleev)
[![Python package](https://github.com/lmmentel/mendeleev/actions/workflows/main.yml/badge.svg)](https://github.com/lmmentel/mendeleev/actions/workflows/main.yml)
[![image](https://pepy.tech/badge/mendeleev)](https://pepy.tech/project/mendeleev)
[![DOI](https://zenodo.org/badge/204296088.svg)](https://zenodo.org/badge/latestdoi/204296088)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/lmmentel/mendeleev">
    <img src="docs/source/_static/img/name_and_logo.png" alt="Logo" width="300">
  </a>

  <h3 align="center">Pythonic periodic table of elements</h3>

  <p align="center">
    A package with a convenient python API for accessing various properties
of elements, ions and isotopes in the periodic table of elements.
    <br />
    <br />
    <a href="https://github.com/lmmentel/mendeleev/issues">Report Bug</a>
    ·
    <a href="https://github.com/lmmentel/mendeleev/issues">Request Feature</a>
    ·
    <a href="https://github.com/lmmentel/mendeleev/pulls">Submit a Pull Request</a>
  </p>
</p>

> [!TIP]
> If you're looking for raw data behind ``mendeleev`` have a look at [mendeleev-data](https://github.com/lmmentel/mendeleev-data) project.
> 
> You can find **all data assets** in multiple formats: 
> - csv, 
> - html,
> - json, 
> - sql,
> - markdown.
>
> All releases a tagged with the same version numbers as ``mendeleev``.

<!-- TABLE OF CONTENTS -->
## Table of Contents

- [Table of Contents](#table-of-contents)
- [About the project](#about-the-project)
  - [Interactive web app](#interactive-web-app)
- [Installation](#installation)
- [Documentation](#documentation)
- [Data](#data)
  - [Basic properties](#basic-properties)
  - [Standardized colors schemes](#standardized-colors-schemes)
  - [Size related properties](#size-related-properties)
  - [Electronegativity scales](#electronegativity-scales)
  - [Descriptive properties](#descriptive-properties)
  - [Physical properties](#physical-properties)
  - [Computed properties](#computed-properties)
  - [Isotope properties](#isotope-properties)
- [Getting started](#getting-started)
  - [Lists of elements](#lists-of-elements)
    - [Isotopes](#isotopes)
  - [Accesing data tables and the database](#accesing-data-tables-and-the-database)
  - [Command line interface utility](#command-line-interface-utility)
- [Contributing](#contributing)
  - [Issues](#issues)
  - [Pull requests](#pull-requests)
- [Implementations in other languages](#implementations-in-other-languages) 
- [License](#license)
- [Citing](#citing)
- [Funding](#funding)

---

source: [https://github.com/lmmentel/mendeleev](https://github.com/lmmentel/mendeleev)

---

## About the project

This package provides a convenient python API for accessing various
properties of elements, ions and isotopes in the periodic table of
elements.

Moreover it provides an easy to use interface to
[pandas](http://pandas.pydata.org/) and convenient visualization
functionality through [bokeh](http://bokeh.pydata.org/en/latest/) that
enables you to create customized periodic tables displaying various
properties.

![peridic_table](docs/source/_static/img/mendeleev_periodic_series.png)

The package also facilitates the exploration and visualization of
periodic trends in the periodic table. If you want to
look at some examples there are a few
[tutorials](http://mendeleev.readthedocs.io/en/stable/tutorials.html)
available as [jupyter notebooks](http://jupyter.org/).

### Interactive web app

If you would like to explore the data available in
[mendeleev](http://mendeleev.readthedocs.org) check out the interactive
web app at [mendeleev.herokuapp.com](http://mendeleev.herokuapp.com/)
where you can create your own periodic tables and visualize the
relations between various properties of elements.

![Periodic table view](docs/source/_static/img/mendeleevapp_periodic.png)

![Correlations view](docs/source/_static/img/mendeleevapp_correlations.png)

## Installation

The preferred installation method is with
[conda](https://conda.io/docs/intro.html) and you can install the package from
the [conda-forge Anaconda channel](https://anaconda.org/conda-forge/mendeleev)
channel by

``` {.sourceCode .bash}
conda install conda-forge::mendeleev
```

The package can also be installed using
[pip](https://pypi.python.org/pypi/pip)

``` {.sourceCode .bash}
pip install mendeleev
```
or [pipenv](https://pipenv.readthedocs.io/en/latest/)

``` {.sourceCode .bash}
pipenv install mendeleev
```

You can also install the most recent version from the project:

``` {.sourceCode .bash}
pip install git+https://github.com/lmmentel/mendeleev.git
```

## Documentation

Full documentation is hosted on [Read the Docs](http://mendeleev.readthedocs.org/en/latest/).

**Key Documentation Pages:**
- [API Overview](https://mendeleev.readthedocs.io/en/stable/api_overview.html) - Architecture and usage patterns
- [Units Support](https://mendeleev.readthedocs.io/en/stable/units.html) - Working with physical units (v1.3.0+)
- [FAQ](https://mendeleev.readthedocs.io/en/stable/faq.html) - Frequently asked questions
- [Troubleshooting](https://mendeleev.readthedocs.io/en/stable/troubleshooting.html) - Common issues and solutions

**Interactive Tutorials:**

There are also tutorials available as [Jupyter](https://jupyter.org/)
notebooks on [binder](https://mybinder.org/) where you can explore the examples interactively:

- [Quick

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Python** (manifests: pyproject.toml, poetry.lock; scanned in UPSTREAM_CLONE)
- Top-level source layout: `alembic/`, `conda-recipe/`, `mendeleev/`, `notebooks/`, `tests/`
- Snapshot size: **184 files**, **7353 lines of code** (measured; see Benchmarks)
- Primary languages: `.py` (88), `.rst` (34), `.png` (20), `.ipynb` (12), `.md` (6), `(none)` (5)
- Upstream commit pinned for this packaging: `bd4716bff94c7acf22210d6ffb75dbd1fcc4f9bc`

---

## Installation

- [Documentation](#documentation)
- [Data](#data)
  - [Basic properties](#basic-properties)
  - [Standardized colors schemes](#standardized-colors-schemes)
  - [Size related properties](#size-related-properties)
  - [Electronegativity scales](#electronegativity-scales)
  - [Descriptive properties](#descriptive-properties)
  - [Physical properties](#physical-properties)
  - [Computed properties](#computed-properties)
  - [Isotope properties](#isotope-properties)
- [Getting started](#getting-started)
  - [Lists of elements](#lists-of-elements)
    - [Isotopes](#isotopes)
  - [Accesing data tables and the database](#accesing-data-tables-and-the-database)
  - [Command line interface utility](#command-line-interface-utility)
- [Contributing](#contributing)
  - [Issues](#issues)
  - [Pull requests](#pull-requests)
- [Implementations in other languages](#implementations-in-other-languages) 
- [License](#license)
- [Citing](#citing)
- [Funding](#funding)

---

source: [https://github.com/lmmentel/mendeleev](https://github.com/lmmentel/mendeleev)

---

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

- [Lists of elements](#lists-of-elements)
    - [Isotopes](#isotopes)
  - [Accesing data tables and the database](#accesing-data-tables-and-the-database)
  - [Command line interface utility](#command-line-interface-utility)
- [Contributing](#contributing)
  - [Issues](#issues)
  - [Pull requests](#pull-requests)
- [Implementations in other languages](#implementations-in-other-languages) 
- [License](#license)
- [Citing](#citing)
- [Funding](#funding)

---

source: [https://github.com/lmmentel/mendeleev](https://github.com/lmmentel/mendeleev)

---

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

[![Latest version released on PyPI](https://img.shields.io/pypi/v/mendeleev.svg?style=flat-square&label=PyPI%20version)](https://pypi.python.org/pypi/mendeleev)
[![MIT license](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![image](https://anaconda.org/conda-forge/mendeleev/badges/version.svg)](https://anaconda.org/conda-forge/mendeleev)
[![Python package](https://github.com/lmmentel/mendeleev/actions/workflows/main.yml/badge.svg)](https://github.com/lmmentel/mendeleev/actions/workflows/main.yml)
[![image](https://pepy.tech/badge/mendeleev)](https://pepy.tech/project/mendeleev)
[![DOI](https://zenodo.org/badge/204296088.svg)](https://zenodo.org/badge/latestdoi/204296088)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/lmmentel/mendeleev">
    <img src="docs/source/_static/img/name_and_logo.png" alt="Logo" width="300">
  </a>

  <h3 align="center">Pythonic periodic table of elements</h3>

  <p align="center">
    A package with a convenient python API for accessing various properties
of elements, ions and isotopes in the periodic table of elements.
    <br />
    <br />
    <a href="https://github.com/lmmentel/mendeleev/issues">Report Bug</a>
    ·
    <a href="https://github.com/lmmentel/mendeleev/issues">Request Feature</a>
    ·
    <a href="https://github.com/lmmentel/mendeleev/pulls">Submit a Pull Request</a>
  </p>
</p>

> [!TIP]
> If you're looking for raw data behind ``mendeleev`` have a look at [mendeleev-data](https://github.com/lmmentel/mendeleev-data) project.
> 
> You can find **all data assets** in multiple formats: 
> - csv, 
> - html,
> - json, 
> - sql,
> - markdown.
>
> All releases a tagged with the same version numbers as ``mendeleev``.

<!-- TABLE OF CONTENTS -->

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Python |
| Manifests detected | pyproject.toml, poetry.lock |
| Files in snapshot | 184 |
| Lines of code | 7353 |
| Dependency references | 2 |
| Dependencies by ecosystem | pypi: 2 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| pypi | sqlalchemy | >=1.3.0 | setup.py |
| pypi | element.py | = mendeleev.cli:clielement | setup.py |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

- [Ions](https://mybinder.org/v2/gh/lmmentel/mendeleev/master?filepath=docs%2Fsource%2Fnotebooks%2Fions.ipynb)
- [Visualizations](https://mybinder.org/v2/gh/lmmentel/mendeleev/master?filepath=docs%2Fsource%2Fnotebooks%2Fvisualizations.ipynb)
- [Advanced visualizations](https://mybinder.org/v2/gh/lmmentel/mendeleev/master?filepath=docs%2Fsource%2Fnotebooks%2Fadvanced_visualizations.ipynb)

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

<!-- omit in toc -->
# Contributing to mendeleev

First off, thanks for taking the time to contribute! ❤️

All types of contributions are encouraged and valued. See the [Table of Contents](#table-of-contents) for different ways to help and details about how this project handles them. Please make sure to read the relevant section before making your contribution. It will make it a lot easier for us maintainers and smooth out the experience for all involved. The community looks forward to your contributions. 🎉

> And if you like the project, but just don't have time to contribute, that's fine. There are other easy ways to support the project and show your appreciation, which we would also be very happy about:
> - Star the project
> - Share it over social media
> - Refer this project in your project's readme
> - Mention the project at local meetups and tell your friends/colleagues
> - Cite the project in academic papers if you've used it in your research

<!-- omit in toc -->
## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [I Have a Question](#i-have-a-question)
  - [I Want To Contribute](#i-want-to-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Your First Code Contribution](#your-first-code-contribution)
  - [Improving The Documentation](#improving-the-documentation)
- [Styleguides](#styleguides)
  - [Commit Messages](#commit-messages)

## Code of Conduct

This project and everyone participating in it is governed by the
[mendeleev Code of Conduct](https://github.com/lmmentel/mendeleev/blob/CODE_OF_CONDUCT.md).
By participating, you are expected to uphold this code. Please report unacceptable behavior
to @lmmentel.

## I Have a Question

> If you want to ask a question, we assume that you have read the available [Documentation](https://mendeleev.readthedocs.io/).

Before you ask a question, it is best to search for existing [Discussions](https://github.com/lmmentel/mendeleev/discussions) that might help you. In case you have found a suitable thread and still need clarification, you can write your question in this thread. It is also advisable to search the internet for answers first.

If you then still feel the need to ask a question and need clarification, we recommend the following:

- Open an [Discussion](https://github.com/lmmentel/mendeleev/discussions/new/choose).
- Provide as much context as you can about what you're running into.
- Provide project and platform versions (oper

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text

The MIT License (MIT)

Copyright (c) 2015 Lukasz Mentel

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `MENDELEEV` (category: CHEMICAL MANUFACTURING)
- **Upstream URL:** https://github.com/lmmentel/mendeleev
- **Pinned commit (SHA):** `bd4716bff94c7acf22210d6ffb75dbd1fcc4f9bc`
- **Branch:** master
- **Pin provenance:** GitHub API commits/master. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`5bf3a5a7aee6733062a540bad631d8c19b90d813605e244521183b0943713b5d`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.


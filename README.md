<div align="center">

# 🔥 PROJECT_NAME

**One-line description of what this repo does.**

[![CI](https://github.com/os-fiscal-de-rejunte/REPO_NAME/actions/workflows/ci.yml/badge.svg)](https://github.com/os-fiscal-de-rejunte/REPO_NAME/actions/workflows/ci.yml)
[![Release](https://img.shields.io/github/v/release/os-fiscal-de-rejunte/REPO_NAME?sort=semver)](https://github.com/os-fiscal-de-rejunte/REPO_NAME/releases)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-fe5196?logo=conventionalcommits&logoColor=white)](https://www.conventionalcommits.org)
[![NASA Space Apps 2026](https://img.shields.io/badge/NASA-Space%20Apps%202026-0B3D91?logo=nasa&logoColor=white)](https://www.spaceappschallenge.org)

</div>

> 📌 **After creating from the template:** replace `PROJECT_NAME` / `REPO_NAME`, update `package-name` in `release-please-config.json` and `name` in `pyproject.toml`, then delete this note.

## Overview

**Challenge:** Harmonization of MODIS and VIIRS Hot Spots
**Problem:** ...
**Solution:** ...

<!-- GIF or screenshot of the demo here -->

## Quickstart

```bash
git clone https://github.com/os-fiscal-de-rejunte/REPO_NAME.git
cd REPO_NAME
cp .env.example .env              # add your FIRMS_MAP_KEY
python -m venv .venv && source .venv/bin/activate
pip install -e ".[dev]"
pre-commit install --hook-type pre-commit --hook-type commit-msg
pytest
```

## Project structure

```
src/         # source code
tests/       # tests
notebooks/   # exploration (outputs cleared before commit)
data/
  sample/    # small, versioned samples
  raw/       # ignored by git
docs/        # documentation and pitch material
```

## Data & methodology

| Source | Product | Use |
|---|---|---|
| NASA FIRMS | MODIS C6.1 (Terra/Aqua) | 2000–present hotspots |
| NASA FIRMS | VIIRS 375 m (S-NPP, NOAA-20, NOAA-21) | 2012–present hotspots |

Limitations: harmonized values are model estimates, not observations. A missing detection does not mean zero fire.

## Contributing

Branch, commit and PR rules: [CONTRIBUTING.md](https://github.com/os-fiscal-de-rejunte/.github/blob/main/CONTRIBUTING.md).

```
git switch -c feat/12-short-description
git commit -m "feat(pipeline): add FIRMS archive ingestion"
```

## Team

Built by **[Os Fiscal de Rejunte](https://github.com/os-fiscal-de-rejunte)** for the NASA Space Apps Challenge 2026, São Paulo.

## License & acknowledgments

[MIT](LICENSE). We acknowledge the use of data and imagery from LANCE FIRMS operated by NASA's Earth Science Data and Information System (ESDIS) with funding provided by NASA Headquarters.

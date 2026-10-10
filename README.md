# vigil

A regex-based secrets scanner written in Python. Built as a learning project.

> **Status:** v1 in progress. Not yet published.

## Scope

| Version | Goal                                                              | Status  |
|---------|-------------------------------------------------------------------|---------|
| v1      | Single-file scanner: AWS access key ID + `password = "..."`       | Started |
| v2      | Test file of tricky inputs (should-match and shouldn't-match)     | Planned |
| v3      | Directory scan honouring `.gitignore`                             | Planned |
| v4      | Git pre-commit hook scanning staged changes only                  | Planned |

## Output

Each finding reports:

- file path
- line number
- pattern name

Matched secret values are deliberately **not** printed.

## Exit codes

- TODO: define what 0 and non-zero mean (the v4 hook depends on this)

## Known limitations

- TODO: list what the patterns deliberately don't match, and why

## Rules for this repo

- Dummy credentials only. No real secrets in code, tests, or docs.
- Package name checked on PyPI and GitHub before any publishing.
- Small, frequent commits.

## Usage

TODO: add once v1 runs.
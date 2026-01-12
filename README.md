# Test Case: Pipenv Basic Sanity

## Package Manager
Pipenv (pip-based)

## Python Version Detection
- **Source**: Pipfile [requires] python_version
- **Expected Version**: 3.10

## Files Present
- Pipfile - Pipenv manifest with python_version = "3.10"
- Pipfile.lock - Pipenv lock file

## Dependencies
- requests==2.31.0
- django==2.2.0
- flask==2.2.5

## Test Purpose
**Basic sanity test for Pipenv** - validates Pipfile version detection.
Tests standard Pipenv project with no conflicts or edge cases.

## Expected Behavior
- Tool detects Pipenv project (Pipfile + Pipfile.lock present)
- Reads python_version from [requires] section
- Successfully installs dependencies with Python 3.10

# Northstar Platform

This repository contains a representative implementation of several Atlas platform services used for software design analysis.

The implementation is intentionally incomplete and contains design problems that have accumulated over time. External systems such as authentication, notifications, and reporting have been replaced with simplified local implementations.

## Purpose

Students should use this repository to examine how design principles appear in code, including:

- abstraction and information hiding
- cohesion and coupling
- responsibility assignment
- duplicated validation
- inconsistent error handling
- maintainability and design for change

## Current Engineering Concerns

- `CustomerService` performs too many unrelated responsibilities.
- Validation logic is duplicated across modules.
- Reporting logic is mixed with customer-management logic.
- Services call external dependencies directly.
- Error handling is inconsistent.
- Some behavior is preserved only through characterization tests.

## Running the Tests

```bash
python -m pip install -e ".[dev]"
pytest
```

## Important

Do not assume every design choice in this repository is good. The code is intended to be analyzed, critiqued, and redesigned.

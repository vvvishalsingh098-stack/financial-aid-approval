
# Financial Aid Approval Module

Python module for secure admin financial aid approval, with tests covering risky paths like blank applications and invalid amounts.

## Features
- Explicit `is_blank()` check for `household_income` + `extra_explaination`
- `approve_blanks` flag to control blank app behavior
- Catches `ValueError`/`TypeError` on invalid `dollar_amount`/`percent`, stores in `user_error`
- Structured API responses: `ok`, `skipped_blank`, `error`

## Quick Start
```bash
pip install -r requirements.txt
pytest



# Week 6 Assignment - Safe Functions

- `safe_tools.py` - three functions (`safe_divide`, `safe_number`, `get_field`) that use `try`/`except` so they return a friendly message instead of crashing.
- `README.md` - this file, describing the project and answering the question below.

## Why can the `if` check not catch `abc` on its own?

An `if` check can only test conditions we thought of in advance, and "is this text a valid whole number?" is not something a simple comparison can answer reliably. The text `abc` looks like perfectly valid input until `int()` actually tries to convert it and raises a `ValueError`, so `try`/`except` is needed to catch the error at the moment it happens.


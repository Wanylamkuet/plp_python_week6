# Week 6 Assignment: Error Handling & Debugging

- `safe_tools.py`: Contains utility functions (`safe_divide`, `safe_number`, and `get_field`) protected by try/except exception-handling blocks.
- `README.md`: Documents the repository, file descriptions, and the reasoning behind error handling vs. conditional checks.

### Why an `if` check cannot catch "abc" on its own
An `if` check can only test conditions you anticipate before executing an operation, whereas passing invalid text like `"abc"` into a type conversion function triggers a runtime exception (`ValueError`) rather than a simple boolean failure. A `try/except` block is required to catch and handle that runtime crash gracefully.
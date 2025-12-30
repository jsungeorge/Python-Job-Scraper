# Project Context: Internship Job Scraper

## Goal
Build a Python-based automated tool that scrapes company career pages for "Intern" or "Co-op" roles and sends email alerts.

## Architecture Structure (Strict)
- /src/scrapers/: Contains individual scraper logic for different sites (e.g., greenhouse.py, lever.py).
- /src/notifications/: Contains email logic (SMTP) to send alerts.
- /src/utils/: Helper functions (random_user_agent, logging_config).
- /data/: Stores the output (jobs.csv) and history (to prevent duplicate alerts).
- /tests/: Unit tests for scrapers.

## Tech Stack Rules
- Language: Python 3.9+
- Libraries: requests, beautifulsoup4, pandas, python-dotenv
- Style: Follow PEP 8. Use Type Hinting (def func(x: int) -> str:).
- Error Handling: strictly handle 403 Forbidden and Network Errors.

## Constraint
DO NOT put all code in main.py. Keep modules separated by responsibility.
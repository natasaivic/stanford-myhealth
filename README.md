# stanford-myhealth

This QA automation project uses Pytest and Selenium to test key user-facing features of the Stanford MyHealth patient portal. The focus is on verifying core functionality such as secure login, dashboard visibility, upcoming appointments, and access to lab results.

## Setup

1. **Create and activate virtual environment:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure environment:**
   - Copy `.env` file and update with your test environment settings
   - Update test credentials (never commit real credentials)

## Running Tests

```bash
# Run all tests
pytest

# Run with verbose output
pytest -v

# Run specific test file
pytest tests/test_login.py

# Run tests matching keyword
pytest -k "login"

# Generate HTML test report
pytest --html=reports/report.html
```

## Project Structure

- `venv/` - Virtual environment (excluded from git)
- `tests/` - Test files (to be implemented)
- `pages/` - Page Object Model classes (to be implemented)
- `utils/` - Utility functions (to be implemented)
- `config/` - Configuration files (to be implemented)
- `reports/` - Test reports and screenshots
- `requirements.txt` - Python dependencies
- `.env` - Environment configuration (not committed to git)

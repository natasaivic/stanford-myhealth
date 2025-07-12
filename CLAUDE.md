# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a QA automation project using Pytest and Selenium to test key user-facing features of the Stanford MyHealth patient portal. The focus is on verifying core functionality such as secure login, dashboard visibility, upcoming appointments, and access to lab results.

## Development Commands

### Environment Setup
- `source venv/bin/activate` - Activate virtual environment
- `deactivate` - Deactivate virtual environment
- `pip install -r requirements.txt` - Install dependencies
- `pip freeze > requirements.txt` - Update requirements file

### Testing Commands
- `pytest` - Run all tests
- `pytest -v` - Run tests with verbose output
- `pytest tests/test_login.py` - Run specific test file
- `pytest -k "login"` - Run tests matching keyword
- `pytest --html=reports/report.html` - Generate HTML test report
- `pytest --screenshot-on-failure` - Take screenshots on test failures

## Project Structure

Current structure:
- `venv/` - Virtual environment (excluded from git)
- `requirements.txt` - Python dependencies
- `.env` - Environment configuration (not committed to git)
- `.gitignore` - Git exclusions

To be implemented:
- `tests/` - Test files for different portal features (login, dashboard, appointments, lab results)
- `pages/` - Page Object Model classes for web elements
- `utils/` - Utility functions for common test operations
- `config/` - Configuration files for test environments and browser settings
- `reports/` - Test reports and screenshots

## Environment Configuration

The `.env` file contains configuration for:
- Test environment URLs (BASE_URL, STAGING_URL, DEV_URL)
- Browser settings (BROWSER, HEADLESS, window dimensions)
- Test credentials (placeholder values only)
- Screenshot and reporting settings

## Testing Guidelines

- Tests target the Stanford MyHealth patient portal user interface
- Focus areas: secure login, dashboard visibility, upcoming appointments, lab results access
- Use Selenium WebDriver for browser automation
- Follow Page Object Model pattern for maintainable test code
- Ensure tests work across different browsers and environments
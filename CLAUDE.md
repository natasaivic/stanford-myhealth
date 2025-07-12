# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a QA automation project using Pytest and Selenium to test key user-facing features of the Stanford MyHealth patient portal. The focus is on verifying core functionality such as secure login, dashboard visibility, upcoming appointments, and access to lab results.

## Development Commands

Since this project uses Pytest and Selenium for testing (as described in README.md), the following commands will likely be relevant once implemented:

- `pytest` - Run all tests
- `pytest -v` - Run tests with verbose output
- `pytest tests/test_login.py` - Run specific test file
- `pytest -k "login"` - Run tests matching keyword
- `pytest --html=report.html` - Generate HTML test report (if pytest-html is used)

For dependency management:
- `pip install -r requirements.txt` - Install dependencies (once requirements.txt is created)
- `pip freeze > requirements.txt` - Update requirements file

## Project Structure (To Be Implemented)

Based on the project description, the typical structure would include:
- Test files for different portal features (login, dashboard, appointments, lab results)
- Page Object Model classes for web elements
- Configuration files for test environments and browser settings
- Utility functions for common test operations
- Test data and fixtures

## Testing Guidelines

- Tests target the Stanford MyHealth patient portal user interface
- Focus areas: secure login, dashboard visibility, upcoming appointments, lab results access
- Use Selenium WebDriver for browser automation
- Follow Page Object Model pattern for maintainable test code
- Ensure tests work across different browsers and environments
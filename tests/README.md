# Mini-SIEM Test Suite

This directory contains test cases for the Mini-SIEM system.

## Test Structure

- `unit/` - Unit tests for individual components
- `integration/` - Integration tests
- `performance/` - Performance and load tests
- `fixtures/` - Test data and mock events

## Running Tests

```bash
# Run all tests
python -m pytest tests/

# Run specific test category
python -m pytest tests/unit/
python -m pytest tests/integration/

# Run with coverage
python -m pytest --cov=src tests/
```

## Test Data

The `fixtures/` directory contains sample log data and events for testing various scenarios.
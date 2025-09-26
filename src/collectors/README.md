# Log and Event Collection Modules

This directory contains modules for collecting logs and events from various sources.

## Modules

- `syslog_collector.py` - Collects syslog events
- `file_collector.py` - Monitors log files for changes
- `network_collector.py` - Captures network events
- `windows_collector.py` - Windows Event Log collection
- `api_collector.py` - Collects events via REST APIs

## Configuration

Collectors are configured through the main config file under the `collectors` section.
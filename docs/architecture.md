# Mini-SIEM Architecture

## System Overview

The Mini-SIEM system is designed with a modular architecture consisting of the following components:

## Core Components

### 1. Collectors (`src/collectors/`)
- **Purpose**: Collect logs and events from various sources
- **Sources**: System logs, application logs, network events
- **Formats**: Syslog, JSON, CSV, custom formats

### 2. Analyzers (`src/analyzers/`)
- **Purpose**: Process and analyze collected data
- **Features**: Pattern matching, correlation, anomaly detection
- **Rules**: Configurable detection rules and filters

### 3. Storage (`src/storage/`)
- **Purpose**: Store and index processed events
- **Options**: File-based storage, database integration
- **Features**: Data retention, compression, indexing

### 4. Visualization (`src/visualization/`)
- **Purpose**: Present data through dashboards and reports
- **Features**: Real-time monitoring, historical analysis
- **Interface**: Web-based dashboard

### 5. Alerts (`src/alerts/`)
- **Purpose**: Generate and manage security alerts
- **Features**: Threshold-based alerts, escalation rules
- **Outputs**: Email, webhook, dashboard notifications

## Data Flow

1. **Collection**: Events are collected from various sources
2. **Processing**: Raw events are parsed and normalized
3. **Analysis**: Processed events are analyzed for threats
4. **Storage**: Events and analysis results are stored
5. **Visualization**: Data is presented through dashboards
6. **Alerting**: Suspicious activities trigger alerts

## Configuration

All components are configurable through files in the `config/` directory.
# Mini-SIEM Example Use Cases

This directory contains example configurations and use cases for different security monitoring scenarios.

## Available Examples

### 1. Basic Web Server Monitoring (`web_server/`)
- Monitor Apache/Nginx access logs
- Detect common web attacks (SQL injection, XSS)
- Track suspicious user agents
- Monitor for file upload attempts

### 2. Windows Domain Monitoring (`windows_domain/`)
- Monitor Windows Event Logs
- Detect failed login attempts
- Track privilege escalations
- Monitor for lateral movement

### 3. Network Security Monitoring (`network_security/`)
- Monitor network traffic patterns
- Detect port scans and reconnaissance
- Track data exfiltration attempts
- Monitor DNS queries for malicious domains

### 4. File Integrity Monitoring (`file_integrity/`)
- Monitor critical system files
- Detect unauthorized modifications
- Track file access patterns
- Alert on sensitive file access

### 5. Cloud Environment Monitoring (`cloud_monitoring/`)
- Monitor AWS/Azure logs
- Detect unusual API calls
- Track resource usage anomalies
- Monitor for privilege escalations

## How to Use Examples

1. Copy the example configuration to your config directory
2. Modify paths and settings for your environment
3. Start Mini-SIEM with the example configuration
4. Generate test events using provided scripts

## Test Event Generation

Each example includes scripts to generate realistic test events for learning and testing purposes.
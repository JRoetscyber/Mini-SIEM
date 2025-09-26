# Mini-SIEM Setup Guide

## Prerequisites

- Python 3.8 or higher
- pip package manager
- 4GB RAM minimum
- 10GB disk space

## Installation

### 1. Clone the Repository
```bash
git clone <repository-url>
cd Mini-SIEM
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Configuration

#### Basic Configuration
1. Copy example configuration files:
   ```bash
   cp config/config.example.yaml config/config.yaml
   ```

2. Edit `config/config.yaml` to match your environment:
   - Set data directories
   - Configure log sources
   - Set alert thresholds

#### Database Setup (Optional)
For enhanced storage capabilities:
```bash
# Install database dependencies
pip install -r requirements-db.txt

# Initialize database
python src/storage/init_db.py
```

### 4. Start the System

#### Development Mode
```bash
python main.py --dev
```

#### Production Mode
```bash
python main.py --config config/config.yaml
```

## Verification

1. Check system status:
   ```bash
   curl http://localhost:8080/status
   ```

2. Access web dashboard:
   - Open browser to `http://localhost:8080`
   - Default credentials: admin/admin

## Troubleshooting

### Common Issues

1. **Port conflicts**: Change port in config file
2. **Permission errors**: Ensure write access to data directories
3. **Missing dependencies**: Run `pip install -r requirements.txt`

### Logs
System logs are available in:
- `logs/mini-siem.log` - Main system log
- `logs/error.log` - Error log
- `logs/debug.log` - Debug information (dev mode)

## Next Steps

- Review `docs/learning_resources.md` for learning materials
- Check `examples/` for sample configurations
- Run tests with `python -m pytest tests/`
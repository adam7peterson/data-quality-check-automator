# Data Quality Check Automator

A comprehensive data quality automation tool supporting Excel, SQL, and Python data sources with automated checks, reporting, and alerts.

## Features

### 1. Data Source Connectors
- Excel file reader (.xlsx, .xls)
- SQL database connector (PostgreSQL/MySQL)
- Python DataFrame handler (Pandas)

### 2. Quality Check Engine
- Null value detection and reporting
- Duplicate record identification
- Outlier detection using statistical methods
- Data type consistency validation
- Range checks for numerical values

### 3. Reporting System
- Generate detailed quality reports in HTML/PDF
- Historical tracking of data quality metrics
- Visualization of quality trends
- Export capabilities for findings

### 4. Cleaning Recommendations
- Automated suggestions for data cleaning
- Best practice recommendations
- Code snippets for common cleaning tasks

### 5. Alert System
- Email notification setup
- Configurable alert thresholds
- Custom alert rules
- Alert history tracking

## Installation

```bash
# Clone the repository
git clone https://github.com/adam7peterson/data-quality-check-automator.git
cd data-quality-check-automator

# Install dependencies
pip install -r requirements.txt
```

## Quick Start

```python
from dqchecker import DataQualityChecker

# Initialize checker
checker = DataQualityChecker()

# Load data
checker.load_excel('your_file.xlsx')

# Run quality checks
report = checker.run_checks()

# Generate report
report.export('quality_report.html')
```

## Project Structure

```
data-quality-check-automator/
├── dqchecker/
│   ├── __init__.py
│   ├── core.py
│   ├── connectors/
│   │   ├── __init__.py
│   │   ├── excel.py
│   │   ├── sql.py
│   │   └── pandas.py
│   ├── checks/
│   │   ├── __init__.py
│   │   └── quality_check.py
│   ├── reporting/
│   │   ├── __init__.py
│   │   └── report.py
│   └── alerts/
│       ├── __init__.py
│       └── alert.py
├── tests/
│   ├── __init__.py
│   └── test_core.py
├── docs/
│   ├── README.md
│   ├── configuration.md
│   └── api.md
├── requirements.txt
├── setup.py
└── README.md
```

## Documentation

See the [docs](docs/README.md) directory for detailed documentation.

## Configuration

See [configuration guide](docs/configuration.md) for setup instructions.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Create a Pull Request

## License

This project is licensed under the MIT License.
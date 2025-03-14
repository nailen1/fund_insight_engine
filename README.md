# Fund Insight Engine

A Python package providing utility functions for fund code management and analysis. This package helps streamline the process of handling fund-related data and provides insights into fund operations.

## Features

- Fund code retrieval and validation
  - Support for various fund types (equity, mixed, bond, etc.)
  - Fund class categorization (mother fund, general, class fund)
  - Division-based fund code management
- Integration with financial dataset preprocessing
- AWS S3 integration for data storage

## Installation

You can install the package using pip:

```bash
pip install fund-insight-engine
```

## Requirements

- Python >= 3.7
- financial_dataset_preprocessor >= 0.2.9
- aws_s3_controller >= 0.7.5

## Usage

```python
from fund_insight_engine import fund_codes_retriever

# Get fund codes by type
equity_funds = fund_codes_retriever.get_fund_codes_equity_type()
mixed_funds = fund_codes_retriever.get_fund_codes_equity_mixed_type()

# Get fund codes by class
mother_funds = fund_codes_retriever.get_fund_codes_mother()
class_funds = fund_codes_retriever.get_fund_codes_class()

# Get fund names mapping
fund_names = fund_codes_retriever.get_mapping_fund_names_main()
```

## Version History

### 0.1.0 (Initial Release)
- Basic fund code management functionality
  - Fund type-based retrieval
  - Fund class-based retrieval
  - Division-based management
- AWS S3 integration
- Financial dataset preprocessing integration

## License

This project is licensed under the MIT License.

## Author

Juneyoung Park (juneyoungpaak@gmail.com)

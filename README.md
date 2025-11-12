# UK Rent Sensitivity Table Calculator

A Python tool for calculating rent sensitivity analysis for UK rental properties, including tax implications, National Insurance, and management fees.

## Overview

This calculator generates a comprehensive rent sensitivity table showing the net monthly income for different rent levels, accounting for:
- Management fees (15%)
- Bills and service charges
- Mortgage payments
- Income tax (40% rate)
- National Insurance (8% rate)
- Mortgage interest tax credit (20%)

## Requirements

- Python 3.13+
- pandas
- numpy
- openpyxl

## Installation

1. Clone the repository:
```bash
git clone https://github.com/sdesyllas/uk-rent-sensitivity-table-calculator.git
cd uk-rent-sensitivity-table-calculator
```

2. Create and activate a virtual environment:
```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

3. Install dependencies:
```powershell
pip install pandas numpy openpyxl
```

## Usage

Run the calculator:
```powershell
python table-generator
```

This will generate an Excel file `rent_sensitivity_barking_riverside.xlsx` with rent sensitivity analysis from £2,200 to £2,700 in £50 increments.

## Output

The generated Excel file includes the following columns:
- Rent (£)
- Management Fee (£)
- Taxable Profit (£)
- Income Tax (£)
- NI (£)
- Total Tax Liability (£)
- Net Monthly Income (£)

## Configuration

You can modify the constants in the `table-generator` file to customize the calculation:
- `mortgage_payment`: Monthly mortgage payment
- `bills`: Monthly bills
- `service_charge`: Monthly service charge
- `mortgage_interest`: Monthly mortgage interest
- `income_tax_rate`: Income tax rate (default: 40%)
- `ni_rate`: National Insurance rate (default: 8%)
- `management_fee_rate`: Property management fee rate (default: 15%)
- `rent_levels`: Range of rent values to analyze

## License

See LICENSE file for details.

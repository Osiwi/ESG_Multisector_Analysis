# ESG Portfolio Optimization (Multisector ML Analysis)

This project analyzes ESG performance and financial metrics across multiple sectors (Energy, Financial Services, Technology) and applies machine learning to explore portfolio construction, risk/return behavior, and allocation decisions.

## What the notebook does
- Loads sector-level financial and ESG data (Energy, Financial Services, Technology - Social, Technology - Software).
- Combines traditional financial metrics and ESG metrics into a unified dataset.
- Engineers features for sustainability performance, profitability, and stability.
- Compares sector behavior to understand which segments are attractive from both a returns and ESG standpoint.
- Prepares data for downstream tasks such as:
  - portfolio scoring,
  - allocation weighting,
  - risk-aware selection.

## Data privacy
The original Excel files (e.g. `Energy_stock_data.xlsx`, `Financial_Services_stock_data.xlsx`, etc.) contain proprietary sector data and are **not** included in this repository.

To reproduce:
1. Create a local `data/` folder (this folder is intentionally git-ignored).
2. Provide your own equivalents of:
   - `Energy_stock_data.xlsx`
   - `Financial_Services_stock_data.xlsx`
   - `Technology_Social_stock_data.xlsx`
   - `Technology_Software_stock_data.xlsx`
3. Use the following pattern in code:

   ```python
   file_paths = {
       'Energy': 'data/Energy_stock_data.xlsx',
       'Financial Services': 'data/Financial_Services_stock_data.xlsx',
       'Technology_Social': 'data/Technology_Social_stock_data.xlsx',
       'Technology_Software': 'data/Technology_Software_stock_data.xlsx'
   }

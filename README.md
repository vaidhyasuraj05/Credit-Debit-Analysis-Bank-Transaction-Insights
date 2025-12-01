# Credit & Debit Analysis — Bank Transaction Insights (Power BI)

## Project Summary
This project analyzes bank transactions (credits and debits) to identify liquidity leakage, branch and bank performance, seasonal patterns, channel mix, and actionable recommendations to improve profitability. Built using Power BI with ETL in Power Query and measures in DAX.

## Business Case
- Total Credit: ~₹115.03M
- Total Debit: ~₹115.38M
- Net Amount: ~−₹349,864

Key problem: high debits relative to credits leading to a negative net position and missed profitability opportunities on high-volume banks/branches.

## Deliverables
- Power BI report
- Sample dataset
- DAX measures
- Power Query steps
- Presentation deck

## How to run
1. Open `CreditDebitAnalysis.pbix` in Power BI Desktop.
2. If the sample CSV is used, update the data source to `data/transactions_sample.csv`.
3. Refresh the dataset and verify relationships (Date -> Transactions).
4. Use filters on the report to analyze specific banks/branches/quarters.

## Key Insights
1. Net negative balance — requires remediation.
2. High-volume banks need profitability improvements via cross-sell.
3. Branch performance is flat — implement KPIs.
4. Debit spikes in Oct–Dec — plan seasonal retention campaigns.
5. Channel mix evenly distributed — shift to low-cost channels.

## Technical notes
- DAX & Power Query steps in `/dax` and `/powerquery`.
- Data model: Star schema — Fact: Transactions; Dimensions: Date, Bank, Branch, Customer.

## License
MIT


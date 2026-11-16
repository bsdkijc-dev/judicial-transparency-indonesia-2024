# Data Quality Assessment — FY 2024 Audited Financial Statements

* **Overall Completeness:** **100%** of all 8 PDF chunks (pp. 1–1652) were accessed and verified—chunks `1–1200` via direct PDF download and chunks `1201–1652` via Drive text extraction.
* **Numeric Integrity:** All 18 CSV files use pure numeric formatting (no currency symbols or thousands separators) and UTF-8 encoding for direct ingestion into Google Sheets, Python, R, and SQL.
* **Key Exceptions Logged (`financial_reconciliation_exceptions_2024.csv`):**
  1. `EXC-2024-001`: SatuDJA vs. SAKTI PNBP estimate discrepancy across 58 satkers.
  2. `EXC-2024-002`: `-Rp 0.16` sub-rupiah rounding difference in Ditjen Badilum *Uang Titipan* (`Bank + Safe` vs. `Closing`).
  3. `EXC-2024-003`: `Rp 1,599.00` January 2024 movement variance in *Biaya Proses* (CaLK F.4.1 p. 189).
  4. `EXC-2024-004`: `Rp 1,533,250,594.00` account-code vs. BMN-code mismatches (16-page register, `PDF6`).
  5. `EXC-2024-005`: `Rp 22,772,000.00` fully paid TGR case (*PA Pekalongan*) awaiting formal BPK removal.
  6. `EXC-2024-006`: `-Rp 156.01B` cross-disclosure scope variance between CaLK F.3 RPL register (**Rp 6.020T**) and CaLK F.4.1 Bank balance (**Rp 6.176T**).

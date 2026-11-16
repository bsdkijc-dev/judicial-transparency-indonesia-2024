# Verification & Reconciliation Protocol — FY 2024

1. **Zero-Fabrication Rule:** Every figure in the 18 CSV datasets is extracted directly from [LKMA2024_AUDITED](https://drive.google.com/drive/folders/1RCxAVq3rPVMYZbeXNIDXcENgbeBN_UUv) or computed explicitly from verified source columns. No missing comparative fields are estimated.
2. **Embedded Image Table Extraction:** Because CaLK Section F.4.1 (*Biaya Proses* and *Uang Titipan Pihak Ketiga*, pp. 189–194) is stored as embedded raster tables inside `LKMA2024_AUDITED-201-400.pdf` (PDF pp. 23–28), all 6 pages were rendered to PNG and visually verified line-by-line.
3. **Cross-Statement Checks Performed:**
   * **Neraca Identity:** `Assets (32,244,542,056,931) - Liabilities (110,776,105,869) = Equity (32,133,765,951,062)` — exact match.
   * **LPE Roll-Forward:** `Opening Equity (31,765,973,920,689) + Deficit-LO (-11,285,885,765,056) + Equity Corrections (-82,698,599,647) + Inter-Entity (11,736,376,395,076) = Closing Equity (32,133,765,951,062)` — exact match.
   * **Grants Sum:** All **656 rows** of `grants_master_register_2024.csv` sum to **Rp 182,722,379,898.00**, matching CaLK F.4.2.1 exactly.
   * **TGR Receivable:** `CaLK F.2` remaining balance (**Rp 18,737,506.00**) matches `CaLK C.1.7` (**Rp 14,989,992.00**) + `CaLK C.3.1` (**Rp 3,747,514.00**) exactly.
   * **KDP Roll-Forward:** `Tabel 52` closing balance (**Rp 475,263,059,024.00**) matches Neraca KDP line exactly.

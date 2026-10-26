# Supply Chain Analytics Using Excel — Companion Files

Companion workbooks and data for the book *Supply Chain Analytics Using Excel*.
All data are **synthetic** and were created for teaching. They do not describe any real organisation.

## Folder structure

```
SupplyChainAnalytics_Excel/
├── data/
│   ├── Meridian_Data.xlsx           Meridian Global Supply data (Excel Tables)
│   ├── meridian_orders_raw.csv      raw orders for the Power Query exercise (Chapter 3)
│   └── meridian_orders_clean.csv    cleaned orders (CSV version)
├── workbooks/                       Start and Completed workbooks, Chapters 2–19
└── cases/
    ├── XL_Ch20_Case_Data.xlsx       coffee cooperative and hospital cases (Chapter 20)
    └── XL_AppC_Synthetic_Data.xlsx  synthetic data generator (Appendix C)
```

## How to use the workbooks

* **Start** workbooks contain the data and layout. Yellow cells without values are the formulas you complete while reading the chapter.
* **Completed** workbooks contain the finished analysis. Use them to check your work.
* Conventions: **blue text on yellow** = input cells; **green** = Solver decision variables; black = formulas.

## Workbooks by chapter

| Ch. | Topic | Workbooks | Add-ins used |
|---|---|---|---|
| 1 | Supply chain analytics and Excel | `data/Meridian_Data.xlsx` | – |
| 2 | Excel essentials | `XL_Ch02_Excel_Essentials_*` | – |
| 3 | Data preparation and KPIs (Power Query) | `XL_Ch03_Data_and_KPIs_*`, `meridian_orders_raw.csv` | Power Query |
| 4 | PivotTables and descriptive statistics | `XL_Ch04_Summarising_*` | Analysis ToolPak |
| 5 | Visualisation | `XL_Ch05_Visualising_*` | – |
| 6 | ABC and XYZ classification | `XL_Ch06_ABC_XYZ_*` | – |
| 7 | Supplier performance, chi-square, scorecards | `XL_Ch07_Supplier_*` | – |
| 8 | t-tests and ANOVA | `XL_Ch08_Comparing_Groups_*` | Analysis ToolPak |
| 9 | Correlation and regression | `XL_Ch09_Regression_*` | Analysis ToolPak |
| 10 | Logistic regression with Solver | `XL_Ch10_Logistic_Solver_*` | Solver |
| 11 | Survey data | `XL_Ch11_Survey_*` | – |
| 12 | Demand forecasting | `XL_Ch12_Forecasting_*` | Solver (optional) |
| 13 | Segmentation and classification | `XL_Ch13_Segmentation_*` | Solver (optional) |
| 14 | Inventory models | `XL_Ch14_Inventory_*` | Goal Seek |
| 15 | Monte Carlo simulation | `XL_Ch15_Simulation_*` | Data Table |
| 16 | Optimisation | `XL_Ch16_Optimisation_*` | Solver |
| 17 | What-if and scenario analysis | `XL_Ch17_WhatIf_*` | Data Table, Scenario Manager |
| 18 | Dashboards | `XL_Ch18_Dashboard_*` | (Power Pivot optional) |
| 19 | Quality and reproducibility | `XL_Ch19_Quality_*` | – |
| 20 | Integrated cases | `cases/XL_Ch20_Case_Data.xlsx` | – |

## Requirements

* Microsoft 365 Excel for Windows is recommended. Most workbooks also work in Excel 2016–2021 and Excel for Mac.
* Functions available only in Microsoft 365 / Excel 2021 (XLOOKUP, FILTER, UNIQUE, SORT, LET, LAMBDA) are practised on separate sheets; all other formulas work in Excel 2010 and later.
* The **Analysis ToolPak** and **Solver** add-ins must be activated once (File → Options → Add-ins → Manage: Excel Add-ins → Go). See Appendix B of the book.

## Notes

* **Chapter 15** uses `RAND()`. Results change on every recalculation; set *Formulas → Calculation Options → Manual* to freeze them. The *Replications* sheet holds recorded results of 500 simulated years per scenario.
* **Chapter 17**: Data Table results are also calculated with direct formulas so that the workbook works in every version. Build the Data Tables yourself as described in the chapter.
* **Solver models** (Chapters 10, 12, 13, 16): the Start workbooks have decision cells at zero (or starting values); the Completed workbooks contain the optimised results.

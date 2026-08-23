# T20 Best XI Analysis

This project uses T20 cricket match and player-performance data to build a role-balanced playing XI from the available dataset. Instead of looking only at total runs or wickets, the analysis prepares separate batting, bowling, and player metrics so that players can be compared according to the role they are expected to perform in the team.

## What the project does

1. Load match, batting, bowling, and player data from JSON files.
2. Clean player names, match identifiers, and other fields used across the datasets.
3. Remove duplicates and records that cannot be used in the analysis.
4. Join the source datasets and create analysis-ready CSV outputs.
5. Calculate batting and bowling measures used to compare players.
6. Group candidates by roles such as openers, middle-order batters, finishers, all-rounders, and specialist bowlers.
7. Use the prepared metrics in Power BI to compare candidates and build the final XI.

## Technologies

- Python
- Jupyter Notebook
- Pandas
- JSON and CSV processing
- Power BI
- DAX

## Project resources

| Resource | Description | Link |
| --- | --- | --- |
| `t20_csv_files` | Final processed CSV files used by the visualization and selection analysis. | [Open folder](https://drive.google.com/drive/folders/104h0Epc5-5VLfSKy-WogzkwuAHIT0K5q?usp=sharing) |
| `t20_json_files` | Source JSON datasets used by the notebook. | [Open folder](https://drive.google.com/drive/folders/1tj3f60kqkleOtJoc6fe93k8wnPpjYD-t?usp=sharing) |
| `DAX Measures and Calculated Columns.xlsx` | Measures and calculated-column formulas used in the Power BI part of the project. | [Open workbook](https://docs.google.com/spreadsheets/d/1tTe3xqlWu1wFkvoj1MioohuJs7bf1Cfh/edit?usp=sharing&ouid=114840663789662506255&rtpof=true&sd=true) |
| Power BI report | Interactive report containing the visual analysis and final selection views. | [Open report](https://app.powerbi.com/reportEmbed?reportId=ee1d329c-33ae-4c3c-a441-4584b5e37d1b&autoAuth=true&ctid=b4b62109-b5e5-499a-a5da-97f68d962343) |

## Repository contents

```text
.
├── Source Code.ipynb       # Data cleaning, joins, metric preparation, and player analysis
├── t20_json_files/         # Source match/player datasets
├── t20_csv_files/          # Processed datasets used for visualization
├── media/                  # Project figures
└── README.md
```

## Run the analysis

```bash
jupyter notebook "Source Code.ipynb"
```

The notebook creates the prepared datasets that are then consumed by the Power BI analysis.

## References used in the original analysis

1. [ICC Men's T20 World Cup](https://en.wikipedia.org/wiki/ICC_Men%27s_T20_World_Cup)
2. [ESPN](https://www.espn.com/)
3. [Data Analytics in the Game of Cricket: A Novel Paradigm](https://www.sciencedirect.com/science/article/pii/S1877050922008523)
4. [Predicting Optimal Cricket Team using Data Analysis](https://ieeexplore.ieee.org/document/9396861)

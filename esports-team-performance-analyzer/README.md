# BGIS Esports Team Performance Analyzer

## Folder structure
```text
esports-team-performance-analyzer/
├── Esports_Team_Performance_Analyzer.ipynb
├── README.md
├── requirements.txt
└── data/
    └── BGIS_2026_Team_Statistics.csv
```

## Dataset
- CSV: `data/BGIS_2026_Team_Statistics.csv`
- Source: Liquipedia, Battlegrounds Mobile India Series 2026: Team Statistics
- URL: https://liquipedia.net/pubgmobile/Battlegrounds_Mobile_India_Series/2026/Statistics
- Table: Overall / All Maps
- Starter extract: 19 team rows transcribed from the visible overall statistics table.
- Target: `top_5_team` (1 = rank 1–5, 0 = other teams)

This is an educational starter extract, not a complete match-by-match dataset. Verify values against the source page before submission because tournament pages may update.

## Algorithms
- Logistic Regression
- SVM
- KNN
- K-Means (supplementary unsupervised clustering)

## Limitation
Only 19 aggregate rows are included, so metrics will be unstable and cannot support reliable generalization. For a stronger project, gather team-level records for individual matches across multiple stages/seasons. Do not describe this as a dependable pre-tournament predictor.

## Run
From the project root:
```bash
pip install -r requirements.txt
jupyter notebook
```
Open the notebook and run all cells. It loads the CSV using the relative path `data/BGIS_2026_Team_Statistics.csv`. Keep the `data` folder beside the notebook.

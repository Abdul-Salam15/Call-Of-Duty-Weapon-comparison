# Call of Duty Weapon Comparison

A small data-analysis project that compares two **Call of Duty: Mobile** weapons using their in-game stat profile and visualizes the result with a grouped bar chart.

## What this project does

The notebook loads weapon stats from a CSV file and asks for two gun names. It then compares these attributes side-by-side:

- Damage
- Fire Rate
- Mobility
- Accuracy
- Range
- Control

If either weapon name is invalid, the notebook prints a validation message instead of plotting.

## Repository structure

```text
.
├── README.md
└── Call of duty insights/
    ├── COD.ipynb
    └── CODM Weapons.csv
```

## Dataset

The dataset is stored in:

- `Call of duty insights/CODM Weapons.csv`

Columns used by the comparison workflow:

- `GUN NAME`
- `GUN TYPE`
- `DAMAGE`
- `FIRE RATE`
- `ACCURACY`
- `MOBILITY`
- `RANGE`
- `CONTROL`

## Requirements

Use Python 3.9+ and install the plotting/data libraries used in the notebook:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## How to run

1. Open the project folder.
2. Start Jupyter:

   ```bash
   jupyter notebook
   ```

3. Open `Call of duty insights/COD.ipynb`.
4. Run cells in order.
5. When prompted, enter two weapon names exactly as they appear in the CSV (example: `Locus`, `Koshka`).

## Notes

- Weapon names are case-sensitive in the current implementation.
- The notebook expects `CODM Weapons.csv` to be available in the same working context as the notebook.

## Future improvements

- Make weapon lookup case-insensitive.
- Add a dropdown/select UI instead of manual text input.
- Save plots automatically to an output folder.
- Convert notebook logic into a reusable Python script or web app.

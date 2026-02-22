# reserve-dashboard

Live, professional dashboard for Union Parish Reserve Deputy hour tracking.

## Data source
This dashboard reads directly from Google Sheets using the gviz JSON endpoint:

- Sheet ID: `1XKQne56PC_iC317LUWkEyq4xnQ4AineeUko5EGvqkEM`
- GID: `787165735`

## Local preview
```bash
python3 -m http.server 4173
```
Then open `http://localhost:4173`.

> Important: The sheet must be shared as **Anyone with the link can view** for live data to load.

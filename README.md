# Australian Wildfire Dashboard

A small Dash application to explore and visualize Australian wildfire data.

This repository contains a compact Dash app implemented in a single script so you can run and inspect it quickly.

## Contents

- `dash_wildfire.py` — main Dash application script (run this to start the web app).
- `requirements.txt` — dependency list (created/updated from your input).

## Prerequisites

- Python 3.8 or newer (3.10/3.11 recommended)
- pip

## Dependencies

This project requires at least:

- dash
- pandas
- plotly
- httpx (pinned in `requirements.txt` as `httpx==0.20` per your install)

Use the repository's `requirements.txt` to install the packages listed there.

## Installation (PowerShell)

1. Create and activate a virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Install dependencies from `requirements.txt`:

```powershell
pip install -r requirements.txt
```

If you prefer to install only core packages manually:

```powershell
pip install dash pandas plotly
```

## Running the app (PowerShell)

From the repository root run:

```powershell
python dash_wildfire.py
```

The Dash server will print a local URL (for example, `http://127.0.0.1:8050`). Open that URL in your browser.

## Data source

The demo app reads wildfire data from a remote CSV. The data URL used in the script is:

[Historical_Wildfires.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0101EN-SkillsNetwork/Data%20Files/Historical_Wildfires.csv)

## Notes about `requirements.txt`

- `httpx` is pinned to `0.20` because you installed that exact version.
- If you want a fully reproducible set of package versions, activate your virtual environment and run:

```powershell
pip freeze > requirements.txt
```

That will overwrite `requirements.txt` with exact pinned versions; commit the result if you want to reproduce the environment later.

## Troubleshooting

- If the app fails to start, check installed packages with `pip list`.
- If installation of certain packages fails (for example, Geo libraries), you may need system libraries — consult the failing package's documentation.

## Contributing

Small fixes, documentation improvements, or adding tests are welcome. Open a PR with your changes.

## License

This project is licensed under the MIT License — see the [LICENSE](./LICENSE) file for details.

## Contact

Questions or feedback: open an issue in the repository.

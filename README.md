# Multiregional Input-Output Table Domestic Balancing Automation

Public project overview for the MRIO Domestic Balancing Automation app.

The application supports domestic transaction balancing, MRIOT compilation, and domestic change analysis for MRIO production workflows. This public repository contains project documentation and a GitHub Pages site only. It does not contain the private source code, input workbooks, generated outputs, executable builds, or internal data files.

Source code is private. Please contact the maintainer to request access.

## What the App Does

- Extracts domestic transaction seed blocks from full MRIO workbooks.
- Reads reviewed current-year row and column control totals.
- Applies manual balancing rules, including a special F5 treatment.
- Runs ordinary RAS to match domestic row and column controls.
- Produces cell-level growth diagnostics and optional bounded RAS refinement.
- Supports single-country and batch domestic balancing.
- Compiles final domestic blocks into pre-final MRIOT workbooks.
- Runs MRIOT compilation validation checks.
- Compares domestic transaction values between two MRIOT/domestic-table states.
- Produces downloadable review workbooks, summaries, heatmaps, and validation tables.

## Public Documentation

- [Project Overview](docs/project-overview.md)
- [User Guide](docs/user-guide.md)
- [Methodology Summary](docs/methodology-summary.md)
- [Access Request Notes](docs/access-request.md)
- [Approved Interface Screenshots](screenshots/)

## GitHub Pages

This repository is designed to be published with GitHub Pages from the repository root.

After pushing this repository to GitHub:

1. Open the public repository on GitHub.
2. Go to `Settings`.
3. Open `Pages`.
4. Under `Build and deployment`, set `Source` to `Deploy from a branch`.
5. Select branch `main` and folder `/root`.
6. Save.

The site will publish at a URL similar to:

```text
https://ChristianJabagat.github.io/mriot-domestic-balancing-app-public/
```

## What Is Not Included

This public repository intentionally excludes:

- Python source code.
- Uploaded MRIO workbooks.
- Reviewed control-total workbooks.
- Supplemental IOT files.
- Generated Excel, CSV, and ZIP outputs.
- Windows and macOS executable build artifacts.
- Internal testing files and private data.

## Screenshots

The screenshots in this repository show the app interface in a clean light-mode state before any private files are uploaded. They are included only to preview the workflow pages and do not show confidential input data or generated results.

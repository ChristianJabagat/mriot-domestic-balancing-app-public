# User Guide

This guide summarizes how users interact with the MRIO Domestic Balancing Automation app.

## Domestic Balancing

Use this page to produce final balanced domestic transaction tables.

### Inputs

- Previous-year MRIO workbook.
- Country configuration workbook.
- Sector/final-demand configuration JSON.
- Reviewed current-year control-total workbook or workbooks.
- Optional supplemental IOT matrix or matrices for special cases.

### Main Steps

1. Select target year and base MRIO year.
2. Confirm workbook sheet names and layout settings.
3. Upload the required input files.
4. Load configuration.
5. Select one country or selected batch countries.
6. Run balancing.
7. Review validation summary, RAS log, bounded RAS log, growth diagnostics, and remaining growth violations.
8. Download the output workbooks or batch ZIP.

### Main Outputs

- Final balanced view workbook.
- Full domestic balancing workbook.
- Batch ZIP output.
- Consolidated final domestic tables workbook for batch runs.

## Compile MRIOT

Use this page to fill domestic diagonal blocks in a pre-final MRIOT workbook.

### Inputs

- Pre-final MRIOT workbook.
- Final balanced domestic table workbooks, or one consolidated final domestic tables workbook.

### Main Steps

1. Confirm MRIOT year and sheet name.
2. Confirm MRIOT size and label layout settings.
3. Upload the pre-final MRIOT.
4. Upload final domestic table files.
5. Run compilation.
6. Review fill summary and validation check summary.
7. Download the compiled MRIOT and validation workbook.

## Domestic Change Analysis

Use this page to compare domestic transaction values between a base full MRIOT and final domestic tables.

### Inputs

- Base full MRIOT workbook.
- Current/final balanced domestic table workbook or workbooks.

### Main Steps

1. Select base year and current year.
2. Choose single-country or batch comparison mode.
3. Adjust growth and materiality thresholds if needed.
4. Upload the base full MRIOT.
5. Upload current/final domestic table files.
6. Run change analysis.
7. Review matching summary, country summary, heatmap, and top-change tables.
8. Download the change-analysis workbook or per-country workbooks ZIP.

## Access Note

This public guide describes app usage only. The private source repository is shared by maintainer approval.

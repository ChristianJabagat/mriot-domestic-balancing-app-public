# Methodology Summary

This page summarizes the public methodology implemented in the app.

## Domestic Seed

The domestic balancing workflow starts by extracting a country's domestic block from a full MRIO workbook. The block consists of sector rows by same-country intermediate sector columns and same-country final-demand columns.

For special cases, the extracted MRIO seed can be averaged cell by cell with a supplemental IOT matrix that has the same expected domestic dimensions.

## Control Totals

The app reads reviewed row and column control totals from current-year country control-total workbooks. Row controls correspond to domestic sector rows. Column controls correspond to domestic sector and final-demand columns.

## Manual Balancing

Manual balancing scales columns to reviewed column controls before ordinary RAS begins. F5 has a special treatment when its seed/control relationship triggers the project's F5 rule.

## Ordinary RAS

Ordinary RAS alternates row scaling and column scaling until row and column controls are both matched within the selected tolerance.

## Growth Diagnostics

Growth diagnostics compare each final balanced cell with the corresponding seed cell. The app reports growth ratios, bounds, row/column total growth context, exemptions, and flag reasons.

## Bounded RAS Refinement

Bounded RAS is optional. It starts from the ordinary RAS result, selects the most severe non-exempt growth-bound breach, caps that one cell, treats it as fixed, and rebalances the remaining free cells. The process repeats until all active growth issues are handled, the iteration limit is reached, or a dead end is detected.

If a later step reaches a dead end, the app keeps the latest accepted balanced checkpoint.

## MRIOT Compilation Checks

After domestic blocks are filled, the compiler produces validation summaries covering domestic fill status, row and column total checks, import-total checks, blank and negative cell scans, GDP expenditure versus production checks, and domestic-basic-price total checks.

## Domestic Change Analysis

Change analysis compares domestic cells between a base full MRIOT and uploaded current/final domestic tables. It classifies new flows, disappeared flows, sign flips, large increases, large decreases, and row/column growth-context outliers.

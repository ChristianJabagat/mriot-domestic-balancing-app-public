# Project Overview

MRIO Domestic Balancing Automation is a workflow application for domestic transaction balancing, MRIOT compilation, and domestic change analysis.

The public documentation describes the project at a high level. The application source code and internal data remain private.

## Purpose

The project helps automate the domestic balancing segment of MRIO production. It supports users who need to:

- Produce balanced domestic transaction tables for individual countries or selected batches.
- Review whether balanced cells changed materially relative to their seed values.
- Compile final domestic tables into a pre-final MRIOT workbook.
- Compare domestic transaction values between years or between methodology versions.

## Main Workflows

### Domestic Balancing

The Domestic Balancing page extracts a domestic seed matrix from an MRIO workbook, reads reviewed row and column controls, applies manual balancing, runs ordinary RAS, and optionally applies bounded RAS refinement.

### Compile MRIOT

The Compile MRIOT page inserts final balanced domestic tables into matching country diagonal blocks in a pre-final MRIOT workbook, then writes compilation checks.

### Domestic Change Analysis

The Domestic Change Analysis page compares cell-level domestic transactions between a base full MRIOT and uploaded final balanced domestic tables. It produces summaries, review flags, charts, and heatmaps.

## Access

Source code is private. Please contact the maintainer to request repository access.

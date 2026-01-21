# clinicaltrialsR
An R wrapper for the ClinicalTrials.gov API that simplifies access to global clinical trial data.


`clinicaltrialsR` is a lightweight R package that provides programmatic access to the ClinicalTrials.gov API, the world’s largest public registry of clinical studies involving human participants.

The package makes it easy to search, retrieve, and analyze global clinical trial data using simple, tidy R functions.

# Project Overview

ClinicalTrials.gov is maintained by the U.S. National Library of Medicine and contains detailed information on hundreds of thousands of clinical studies worldwide, including:

- Trial titles and descriptions

- Medical conditions and interventions

- Study phases and designs

- Recruitment status

- Enrollment numbers

- Locations and sponsors

- Start and completion dates

The goal of this project is to build a clean API wrapper that allows researchers, students, and analysts to easily explore and analyze this data directly from R.



# What This Package Will Do

This package implements a small but complete client for the ClinicalTrials.gov API.

## 1. Study Discovery & Search

Functions to search clinical trials by keyword, condition, or intervention.

`ct_search_studies(query = NULL, condition = NULL, intervention = NULL, page_size = 100)`

Search for clinical trials using keywords or structured medical filters.

## 2. Trial Retrieval

Functions to retrieve detailed information for specific trials.

`ct_get_study(nct_id)`

Retrieve full metadata for a single clinical trial using its NCT identifier.


## 3. Metadata & Field Discovery

Functions to explore what data fields are available in the API.

`ct_metadata()`

List all available study fields and their definitions.


## 4. Database Statistics

Helper functions to retrieve summary statistics about the clinical trials database.

`ct_stats_field_sizes()`

Show how often different study fields appear.

`ct_stats_field_values(field)`

Retrieve common values for a given field (e.g. Phase, OverallStatus).

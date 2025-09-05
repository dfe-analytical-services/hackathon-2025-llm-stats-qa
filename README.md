# Using LLMs for Third-Line QA on Statistical Releases README

## Introduction

Purpose: The code in this repository was produced as part of the 2025 pre-stats away day Hackathon, for the project "Using LLMs for Third-Line QA on Statistical Releases". It aims to utilise different elements of LLMs at different points in the publication production process to support with summarising trends, comparison of text and underlying data, drawing insights, and quality assuring between the publication and the EES API

Overview: code for different points in the publication production process is held in separate folders. The main contents of this repo are:
1. Data - holds files utilised in notebooks held in the Code folder. Sample csv files are from previous EES publications, and take the form of EES tidy data csv files, accompanying metadata files and a table of headline measures. Also holds commentary in the form of a docx file which is used in the QA_content_underlying_data code
2. Code - holds notebooks relevant to the individual uses of LLMs at different points in the publication process
    - create_narrative_for_characteristics - uses underlying data in csvs to produce a markdown/html summary of characteristic trends
    - QA_content_underlying_data - takes word docs of publication commentary and csv files for corresponding underlying data and runs checks on whether there are any mismatches between the two
    - jt_ai_overview - uses underlying data in csvs and text strings from the associated publication to produce an example summary, to QA the headline summary text using the underlying data, to produce alternative text for tables and a chatbot which could provide answers to user questions on the publication
    - Web_scraping - takes a url for a stats publication and extracts the information to a text file
    - API_LLM_query - uses a LLM to write python code to QA data on the EES API
3. Outputs - holds the outputs from notebooks in the Code folder:
    - Files starting "ebacc_summary" are outputs from create_narrative_for_characteristics
    - aiccessible_table_output.md is the output from jt_ai_overview
    - KS4_performance.txt is the output from Web_scraping
    - api_output.txt is the output from API_LLM_query
4. Archived_code - code which was tested to try and get the LLM to directly query the EES API. Provides useful examples of methods for doing this which were unsuccessful.

## Requirements

-   Access: no access requirements outside of this repository. Sample data files from existing publications are held in the "data" folder of the repo
-   Skills/knowledge: general understanding of Databricks, Python and LLM prompting is beneficial but not required
-   Version control/Renv: version control is managed through the github repository. Packages for individual notebooks are installed and loaded at the head of each notebook

## Getting started

-   Setup instructions: no specific setup is required, all dependencies and packages are installed within the notebooks they are required for
-   Data input/output: sample files can be found in the "data" folder of the repo. Csv data is expected to take the same form as that uploaded to EES for publication production (i.e. a tidy csv data file and accompanying metadata file)

## How to run and update

-   Running the code: notebooks should be run individually and at the appropriate point in the publication process
-   Updating guidelines: prompts within notebooks and data utilised in notebooks may need amending depending on source and desired output
-   Issue reporting: please raise any issues through the "Issues" tab on the github repo

## Contact details

-   Main contacts: Cheena Ghataoura, Daniel Dodgson, Gemma Selby, Jake Tufts, Rebecca Wedge-Roberts
-   Support channels: the pre-stats awayday hackathon teams page has a dedicated LLMs channel which may be a good place to post any questions

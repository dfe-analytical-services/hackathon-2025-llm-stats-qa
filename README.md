# Using LLMs for Third-Line QA on Statistical Releases README

## Introduction

Purpose: The code in this repository was produced as part of the 2025 pre-stats away day Hackathon, for the project "Using LLMs for Third-Line QA on Statistical Releases". It aims to utilise different elements of LLMs at different points in the publication production process to support with summarising trends, comparison of text and underlying data, drawing insights, and quality assuring between the publication and the EES API

Overview: code for different points in the publication production process is held in separate folders. The main contents of this repo are:
1. Data - holds sample csv files utilised in notebooks held in the Code folder. Sample csv files are from the KS4 performance publication, and take the form of an EES tidy data csv, its accompanying metadata file and a table of headline measures.
2. Code - **_(move narrative_section code into here)_** holds notebooks relevant to the individual uses of LLMs at different points in the publication process
    - create_narrative_for_characteristics - uses underlying data in csvs to produce a markdown/html summary of characteristic trends
    - _CHEENA PLEASE INSERT YOUR NOTEBOOK NAME AND WHAT IT DOES HERE_
    - jt_ai_overview - uses underlying data in csvs and text strings from the associated publication to produce an example summary, to QA the headline summary text using the underlying data, to produce alternative text for tables and a chatbot which could provide answers to user questions on the publication
    - Web_scraping - takes a url for a stats publication and extracts the information to a text file
    - API_LLM_query - uses a LLM to write python code to QA data on the EES API
3. Outputs - **_(move scraped_data and narrative section outputs into here)_**
4. Archived_code - code which was tested to try and get the LLM to directly query the EES API. Provides useful examples of methods for doing this which were unsuccessful.

## Requirements

-   Access: no access requirements outside of this repository. Sample data csv files from the KS4 performance publication are held in the "data" folder of the repo
-   Skills/knowledge: general understanding of Databricks, Python and LLM prompting is beneficial but not required
-   Version control/Renv: version control is managed through the github repository. Packages for individual notebooks are installed and loaded at the head of each notebook

## Getting started

-   Setup instructions: *Provide step-by-step instructions on how to set up the environment, including installing dependencies.*
-   Data input/output: sample data csv files can be found in the "data" folder of the repo. Data is expected to take the same form as that uploaded to EES for publication production (i.e. a tidy csv data file and accompanying metadata file)

## How to run and update

-   Running the code: *Explain how users can best run the code, for example by running a run all script.*
-   Updating guidelines: *Outline the process for updating and contributing to the repository, including specific scripts and lines where updates are frequently needed. Describe how to get changes reviewed.*
-   Issue reporting: please raise any issues through the "Issues" tab on the github repo

## Contact details

-   Main contacts: Cheena Ghataoura, Daniel Dodgson, Gemma Selby, Jake Tufts, Rebecca Wedge-Roberts
-   Support channels: the pre-stats awayday hackathon teams page has a dedicated LLMs channel which may be a good place to post any questions

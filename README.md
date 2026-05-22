# Publication_BMJ2026-Mort5to19

Estimates of global causes of death for children and adolescents aged 5-19 in 2000-24

## Developer instructions

-   Clone repository to computer
-   Open `/src/prepare-session/set-inputs`
    -   Set age-sex group for estimation
    -   Set years of estimation
-   Run make file

## Code

Source code is made available in the `src` folder, with sub-folders for each stage of the project pipeline. There is a `make.R` file in the main directory folder which executes code in the correct order. 

Our pipeline consists of seven main stages:

-   `prepare-session`
-   `data-management`
-   `estimation`
-   `prediction`
-   `squeezing`
-   `uncertainty`
-   `results`

## Generated files

Generated files created by running the source code are stored in the `gen` folder. The `/gen` subdirectories match the pipeline stages.

Each subdirectory in `gen` contains the following subdirectories:

-   `input`: any required input files to run this step of the pipeline
-   `temp`: temporary files, such as an Excel dataset that needs to be converted into a CSV
-   `output`: stores the final result of the pipeline stage
-   `audit`: quality checks, diagnostic information on the performance of each step in the pipeline.

## Directory structure

This directory structure was conceptualized using resources from the [Tilburg Science Hub](https://tilburgsciencehub.com/), in accordance with recommended workflow and data management principles for research projects.

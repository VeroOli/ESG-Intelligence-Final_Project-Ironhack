# Final_Proyect
This project aims to create a tool that allows investors and investment advisors to conduct analysis from an ESG (Environmental, Social, and Governance) perspective, generate an ESG score for each company, and review the evolution of their emissions.

Definition of Objectives and Scope

Main Objective: Create a tool to analyze and score companies from an ESG perspective and project their emissions evolution to assess their alignment with the Net Zero 2050 goal.
Scope: Includes data collection, ESG analysis, generation of ESG scores, emission predictions, and evaluation of alignment with Net Zero 2050 objectives.
ESG Definition & Emissions

ESG Components: Environmental, Social, and Governance criteria used by investors to assess the sustainability and ethical impact of investments in a company or asset.
Environmental (E): Evaluates how a company impacts and manages natural resources including energy and water use, carbon emissions, waste management, recycling, and biodiversity protection initiatives.
Social (S): Examines how a company manages relationships with employees, suppliers, customers, and communities, covering labor conditions, worker rights, diversity and inclusion, community impact, product responsibility, and customer satisfaction.
Governance (G): Considers how a company is managed and governed, focusing on board structure, transparency, ethical behavior, legal compliance, and policies against corruption and bribery.
GHG Emissions: Scope 1, Scope 2, and Scope 3 emissions categories.
Solutions

Risk Reduction: Companies meeting ESG criteria are better positioned to face regulations and market changes, reducing long-term financial risks.
Growth Opportunities: Companies with strong ESG practices can capitalize on new market opportunities such as increasing demand for sustainable products.
Reputation: Companies excelling in ESG typically enjoy a better reputation, leading to increased customer loyalty and community relations.
Long-term Profitability: Investments in companies with high ESG scores tend to be more sustainable and potentially more profitable in the long run.
Data Model Analysis

Data Source: Utilizing Bloomberg API, generating various CSV files: companies, dataset, fields, hist_score, hist_scope.
Materiality Mapping: Custom weightings and variable usage based on industry.
Python Transformation: Data cleaning, creating new metrics and relationships, generating tables like merged_data, filtered_merged_data, ESG_score, esg_percentage, environmental, social, governance, materiality, historical_score, historical_scope.
Machine Learning (Prophet): Creating emission projections for upcoming years.
SQLite3 Database

Storing CSV-generated tables into a database.
Power BI

Connecting Power BI to the database, generating a star schema model:
merged_data: Fact table with ISIN key, company-specific data, and industry.
filtered_merged_data: Combined metrics and data from other tables.
ESG: Consolidated table aggregating global ESG scores.
esg_percentage: Percentage data of ESG score.
environmental, social, governance: Specific data tables for each ESG dimension.
historical_scope and historical_score: Historical data on emissions and ESG scores respectively.
projections: Future emission projections.
Selectable Columns: Table enabling selection of specific columns.
Data Architecture

Diagram illustrating data flow and connections.
Next Steps

Expand industries beyond current coverage (Semiconductors, Automobiles, Software).
Further delve into potential risks and opportunities.
Implement portfolio aggregation and scoring capabilities.
Quantify opportunities and risks for incorporation into company valuations.









📁 Folder structure
└── Final_Project
    ├── .gitignore
    ├── README.md
    ├── ESG Intelligence.pbix
    ├── notebooks
    │   ├── others
    │   ├── EDA_v2.ipynb
    │   ├── Materiality.ipynb
    │   ├── Histrical.ipynb
    │   ├── MachineLearning.ipynb
    │   └── SQLite.ipynb
    │   
    │  data
    │    ├── merged_data
    │    ├── ESG_score
    │    ├── enviromental
    │    ├── social
    │    ├── governance
    │    ├── esg_percentage
    │    ├── filtered_merged_data
    │    ├── materiality
    │    ├── historical_score
    │    ├── historical_scope
    │    └── projections
    │ 
    │  database
    │ 
    └── images


        
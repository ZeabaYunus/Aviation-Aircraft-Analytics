# Aviation Aircraft Analytics (Still a work in progress)

## Project Overview

Aviation Aircraft Analytics is a Python-based data analytics and machine learning project focused on analysing aircraft technical and operational characteristics using real-world aviation datasets. The project combines exploratory data analysis, statistical modelling, and predictive analytics to investigate relationships between aircraft dimensions, performance metrics, and operational classifications.
The primary objective of the project is to build a robust analytical framework capable of identifying patterns within aircraft engineering data while also developing predictive models for aircraft performance indicators such as Maximum Take-Off Weight (MTOW). This project was developed using Python within a Jupyter Notebook environment and forms part of a broader aviation analytics portfolio focused on advanced statistical analysis and machine learning applications in the aerospace sector.

### Datasets Used

1. FAA Aircraft Characteristics Database
Primary dataset containing detailed aircraft specifications and operational characteristics for 388 aircraft types.
Key Variables Included
Manufacturer
Aircraft model
Wingspan
Aircraft length
Tail height
Number of engines
Maximum Take-Off Weight (MTOW)
Maximum Landing Weight (MALW)
Parking area requirements
Wake turbulence category
Operational classifications

### Dataset Dimensions

Rows: 388 aircraft types
Columns (original): 56
Columns (after cleaning): 42

### Programming Language

Python

### Libraries Used

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- Development Environment
- Jupyter Notebook

### Project Workflow

#### Phase 1 — Data Import and Initial Inspection

The project began by importing the aircraft dataset into Python using Pandas. Initial inspection involved:

- Viewing dataset dimensions
- Examining column names
- Identifying missing values
- Understanding variable types
- Checking dataset consistency
- This stage established the overall structure and quality of the raw dataset before analysis

#### Phase 2 — Data Cleaning and Preprocessing

Several preprocessing steps were carried out to improve data quality and prepare the dataset for statistical analysis and modelling. Cleaning Tasks Performed removed unnecessary unnamed columns, identified columns with excessive missing values, retained operationally relevant variables
checked for null values across remaining features and verified dataset integrity after cleaning. The cleaned dataset was reduced from 56 to 42 meaningful variables.

#### Phase 3 — Exploratory Data Analysis (EDA)

Exploratory analysis was performed to identify trends and relationships within the aircraft dataset.
Manufacturer Distribution Analysis - A horizontal bar chart was created to analyse the distribution of aircraft manufacturers in the dataset.

Key findings:

- Cessna and Boeing had the largest representation
- Airbus showed strong presence among commercial aircraft
- Regional and business jet manufacturers such as Embraer and Gulfstream were also represented
- The dataset captures both commercial and general aviation sectors

#### Phase 4 — Correlation Analysis

A correlation matrix was developed to investigate relationships between major aircraft characteristics.
Variables analysed were: 

MTOW
Wingspan
Aircraft length
Parking area
Number of engines

Key findings:

- Strong positive correlations were identified between aircraft size variables
- Parking area showed extremely high correlation with MTOW
- Wingspan and length were strongly linked to aircraft weight
- Engine count demonstrated only moderate correlation with aircraft size
- This phase confirmed that aircraft dimensions are strong predictors of overall aircraft mass and operational footprint

#### Phase 5 — Machine Learning Regression Model

A regression model was developed to predict Maximum Take-Off Weight (MTOW) using aircraft geometric and operational variables

- Model Inputs
- Wingspan
- Aircraft length
- Number of engines
- Parking area

Key findings:

The regression model achieved extremely strong predictive performance, explaining approximately 97.6% of the variance in aircraft MTOW. This indicates that aircraft geometric characteristics are highly effective predictors of aircraft weight.

#### Phase 6 — Model Diagnostics and Residual Analysis

Additional visualisations were produced to evaluate model behaviour.

#### Phase 7 — Statistical Hypothesis Testing

A statistical t-test was performed to evaluate significance within the model outputs.

Results:

- T-Statistic: -0.602
- P-Value: 0.550

Interpretation

The large p-value indicates no statistically significant difference within the tested sample distributions at conventional significance levels.


This project will later on expand to: 

- Advanced regression techniques
- Time-series forecasting
- Aircraft delivery prediction models
- Airbus vs Boeing comparative analysis
- Feature importance analysis
- Clustering and aircraft segmentation
- Interactive dashboards
- Predictive operational analytics
- Machine learning optimisation
- Additional aviation datasets integration

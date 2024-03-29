P8105 Data Science I - Finals Project Proposal
================
07 November 2019

# Tentative Title

Our tentative title is: Exploring The Use of Fragility Index outside of
Oncology Drug Development

# Team Members

  - “Bryan Bunning - UNI: bjb2178”
  - “Gavin Ko - UNI: wk2343”
  - “Yuanzhi (Fisher) Yu - UNI: yy3019”
  - “Zongchao Liu - UNI: zl2860”
  - “Kevin S.W. - UNI: ksw2137”

# Motivation

The Fragility Index has been suggested to be an easy-to-understand
metric of a clinical trials’ robustness, which may pair well with other
frequently discussed metrics like p-values. We are interested how the
fragility index may differ based on different clinical trial
characteristics. Multiple papers have shown that it requires just a few
patients to alter outcomes of many large phase III trials. It is of
concern to us that these studies require billions of dollars sunk but
outcomes can be “easily” rendered obsolete based on so few participant
outcomes.

Our main question of interest is whether fragility index is associated
with a disease type. Specifically, we want to test the difference in
fragility index for cancer related therapies to non-oncology immunologic
monoclonal antibodies such as allergy, diabetes, and asthma. As a prior
belief, we hypothesize that the median fragility Index of trials
targeting cancers will be less than trials targeting auto-immune chronic
diseases.

# Intended Final Products

  - Dataset of clinical trials with baseline information and our
    filtering strategy
  - Figures/graphs highlighting our data compared to previously
    published information
  - Statistical test comparing median fragility index based on different
    characteristics
  - Website that collates our findings with landing page, background,
    graphs, data, methods, and FI calculator.

# Anticipated data sources

  - Search engines: Google Scholar, Pubmed, clinicaltrials.gov
      - Review of ~25 trials with inclusion criterias of:
          - Auto-immune disease-related phase 3 RCTs with a pairwise
            primary outcome, uses monoclonal antibody
          - Time period: 2007-2017  
          - Exclude trial designs with complicated trial design or
            mathematical methods
          - Trials are published in a high impact journal e.g. NEJM,
            JAMA
  - After trials are selected, will scrape data from clinicaltrials.gov
    using its API to get csv format and use R for analysis

# Plan for Analysis/Visualization and Challenges

### Analysis

  - Data operation and outcome analysis:
      - Create R function to calculate the fragility index
      - 2-sample analysis for statistical test the difference between
        oncology / non-oncology diseases with their respective fragility
        indexes

### Visualization

  - R ggplot or Plotly or Shiny?

### Potential Challenges

  - Making FI calculator
  - What interactions will be placed (Shiny)
  - Obtaining enough high-quality data
  - Creating FI function

# Planned Timeline

  - Data scraping and processing: ~10 days (11/9/2019)
  - Data analysis, review, graphical construction: ~7 days
  - Web building: ~4 days
  - Debugging: all the time

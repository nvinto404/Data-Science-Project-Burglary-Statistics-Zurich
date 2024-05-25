# Data Science Project-Burglary Statistics Zurich
 *Laura Kunz, Natalie Vintonjak, Yannick Sanner*

**SS 2024 - MSc Wirtschaftsinformatik** 

**Introduction**
In recent years, burglaries and thefts have become a growing concern for the Canton of Zurich and its municipalities. Given this increase, it is crucial to understand the underlying factors that contribute to this problem. This research aims to investigate the dynamics of these crimes since 2009 and explore potential links with various socio-economic variables such as population density, age distribution as well as the economic circumstances of the population.

The background to this project lies in the increasing number of news reports from the police in the canton of Zurich. In an initial analysis, we used NLP techniques to identify various topics in the news feeds of the cantonal police. One topic block shows police activities such as checks and interventions. Another highlights stolen valuables such as watches and jewelry and another block focuses on suspicious activity reports and police interventions.

(Opendata.Swiss, undated; News, undated)

**Overview**
The aim of this research is to gain a better understanding of the dynamics of burglary and sneak-in thefts in the Canton of Zurich and to provide well-founded insights for the development of effective prevention strategies.
The problem statement of this work lies in the need to identify the factors influencing the frequency of burglary and sneak-in thefts. In particular, various socioeconomic variables such as population density, taxable income per capita, and financial assets per capita are examined to uncover potential correlations.

**Research Questions and Hypotheses**
The central research question is: What correlations exist between socioeconomic variables such as population density, taxable income per capita, financial assets per capita, and the frequency of burglary and sneak-in thefts in the municipalities of the Canton of Zurich since 2009?

- **H1**: "The higher the population density of a municipality, the more likely it is that the total number of burglaries will be higher."
- **H2**: "The higher the average taxable income per capita in a municipality, the lower the total number of burglaries in that municipality."
- **H3**: "The higher the financial assets per capita in a municipality in 2022, the higher the number of burglaries and sneak-in thefts in that municipality."
- **H4**: "There could be a correlation between the age distribution of the population and the number of burglaries and sneak-in thefts in municipalities."

**Project Components**
To answer the research question, detailed data analysis and modeling were conducted in Python. Data from various sources were used, including the opendata.swiss platform and the Zurich Cantonal Police news site.

First, data were obtained from the opendata.swiss platform, which includes the number of burglaries as recorded in the Zurich Cantonal Police crime statistics. This data is broken down by municipality and, in the case of Zurich, by city district. Additionally, information on population numbers, demographic and socioeconomic data was used to establish a relation.

It is important to note that the police crime statistics (PKS) of the Canton of Zurich are published annually and only include crimes known to the police. The PKS is an output statistic, meaning the crimes do not appear in the statistics at the time they occur, but only after the police have completed an initial report on the crime.

# Notebooks
1. **[EinbruchDaten.ipynb](./EinbruchDaten.ipynb)**: This notebook scrapes the burglary data via API and saves it into the database.
2. **[Bevoelkerungsdichte_KantonZurich_2009-2023.ipynb](./Bevoelkerungsdichte_KantonZurich_2009-2023.ipynb)**: This notebook scrapes the population density data and saves it into the database.
3. **[BevölkerungnachAlter_KantonZurich_2009-2022.ipynb](./BevölkerungnachAlter_KantonZurich_2009-2022.ipynb)**: This notebook scrapes the age distribution data and saves it into the database.
4. **[FinanzvermoegenKantonZurich.ipynb](./FinanzvermoegenKantonZurich.ipynb)**: This notebook scrapes the financial assets data and saves it into the database.
5. **[SteuerbaresEinkommennatürlicherPersonen_KantonZurich_2009-2022.ipynb](./SteuerbaresEinkommennatürlicherPersonen_KantonZurich_2009-2022.ipynb)**: This notebook scrapes the taxable income data and saves it into the database.
6. **[EDA.ipynb](./EDA.ipynb)**: This notebook contains the Exploratory Data Analysis including correlation matrix, linear regression, box plots, histograms, and violin plots.
7. **[GeoDaten.ipynb](./GeoDaten.ipynb)**: This notebook visualizes the geographical information for the Canton of Zurich and their burglaries for 2022.
8. **[Modellierung.ipynb](./Modellierung.ipynb)**: This notebook contains models such as Random Forest Classification, Time Series Prediction with ARIMA, and Regression Analysis.
9. **[RNN.ipynb](./RNN.ipynb)**: This notebook uses an RNN model to classify new data and assess the criminality risk for municipalities.
10. **[Sentiment.ipynb](./Sentiment.ipynb)**: This notebook scrapes the news feed of the police and uses sentiment analysis as well as other NLP techniques to analyze the data.

**Note**: All cleaned and structured data is saved in the subfolder `Cleaned_CSV_files`.


# Childhood-lead-poisoning-R
Introduction

Childhood lead poisoning is a serious health issue that can damage the brain and nervous system, slowed growth and development, learning and behavior problems and hearing and speech problems. In 2012, CDC established that a blood lead level of 5 mcg/dL is the reference level for exposure to lead in children. This level is used to identify children who have blood lead levels higher than most children's levels. Approximately half a million U.S. children ages 1-5 have blood lead levels above the blood lead value at which CDC recommends public health actions be initiated.

Questions to ask

• What percentage of children are tested positive for higher levels of lead in the US?
• Which geographical type has higher reported cases in New York city?
• Which borough/neighborhood has highest and lowest levels of reported cases in New
York city?
• Is there any increase or decrease in the number of cases based on year?
• Are there any possible trends between the data sets of children tested under 3 years and
children tested under 6years?

Materials/Data sets used

The data sets I selected for this analysis are from NYC OpenData and CDC.gov
1. CDC National Childhood Blood Lead Surveillance
Data: https://www.cdc.gov/nceh/lead/docs/CBLS-National-Table-Update- 042619.xlsx
About this data set: The data shows state-level blood lead test data summarized by state, year, and blood lead level (BLL) group. This table represents data reported by state to the national surveillance system over the past several years (2012-2017). The data represents only a subset of state-specific data and is not a population-based estimate, so we are not able to compare states or generate national prevalence estimates.
2. Children Under 6 yrs with Elevated Blood Lead Levels (BLL)
https://data.cityofnewyork.us/Health/Children-Under-6-yrs-with-Elevated-Blood-
Lead-Leve/tnry-kwh5
About this data set: All NYC children are required to be tested for lead poisoning at around age 1 and age 2, and to be screened for risk of lead poisoning, and tested if at risk, up until age 6. These data are an indicator of children younger than 6 years of age tested in NYC in a given year with blood lead levels of 5 mcg/dL or greater. In 2012, CDC established that a blood lead level of 5 mcg/dL is the reference level for exposure to lead in children. This level is used to identify children who have blood lead levels higher than most children's levels. The reference level is determined by measuring the NHANES blood lead distribution in US children ages 1 to 5 years, and is reviewed every 4 years.
3. Children Tested for Lead by Age 3
https://data.cityofnewyork.us/Health/Children-Tested-for-Lead-by-Age-3/fzh2- sxib
About the Data: All NYC children are required to be tested for lead poisoning at around age 1 and age 2, and to be screened for risk of lead poisoning, and tested if at risk, up until age 6. These data are an indicator of the number and percentage of children turning 3 years old in a given year who were tested for lead poisoning.
How calculated: To identify children tested for lead poisoning, birth records for all children born in New York City to New York City resident mothers, and turning 3 years old in a given year were matched to children tested for lead poisoning before age 3.

Methods

The packages I used for my analysis are dplyr, ggplot2, tidyverse, readxl, openxlsx, data.table, tidyr, zoo, plyr, janitor, base. I have used scatterplots and barplots to visualize distributions for all three data sets. For the first step, I imported data sets which are in cvs and xlsx formats. Next, I checked for missing data. The data sets I have chosen have a sizable amount of missing information. Most of them are columns that are additional notes for the observations which are not useful for the analysis. The CBLS data set had multiple headers. The headers were cleaned and renamed because they are very descriptive and are hard to use them downstream.
Furthermore, the correlation analysis is performed on the Age 6 data set to check for any possible correlations.

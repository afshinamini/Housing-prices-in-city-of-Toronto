# Toronto Housing Prices Project

## Question: Why are houses so expensive in Toronto?
There has been a lot of public debate
recently about housing prices in Toronto. The cost of living is becoming unaffordable for
many Torontonians and home ownership has become unfeasible for a growing
percentage of the population. There have been lots of explanations offered and
solutions presented from across the political spectrum, yet the data underlying many of
these arguments seems surprisingly scarce and the arguments surprisingly
non-quantitative. Using any means accessible to you as a private citizen, and any data
available that you deem relevant, can you propose what you think is the most important
cause of high prices (e.g. lack of supply, lending policy, speculation/foreign ownership,
tax policy etc.). Based on this, what are one or two policy proposals that are most likely
to reduce housing prices by the largest magnitude? (Note: Don’t worry about potential
adverse side effects of such proposals. The goal of the exercise is to come up with a
good simplified model of the housing market, not to come up with policy proposals you
would necessarily vote for.).<br>
<br>
To start answering this question, first we need to determine what parameters affect housing prices in Toronto.<br>
<br>
A study by Royal Bank of Canada and the Pambia Institute indicated following parameters affect housing prices in Toronto:
<br>
* Real income and demographics
* The cost and accessibility of mortgages
* Construction and development costs
* Land availability and regulations
* Location and housing stock supply and demand

Source:<br> 
Pambia Institute:Understanding the factors affecting home prices in the GTA (https://www.pembina.org/pub/2502).<br>
<br>
Data from different sources (cited at the end) where gathered and compiled to take these factors into account in this anaysis:
<br>
* Monthly Home Transactions: database containing monthly house sales information.
* Ontario Employment Wages: Monthly wages across Ontario.
* Land Pricing Index: Land price index in Toronto.
* Mortgage Rates: prime and mortgage retes.
* Average Residential Building Construction Price Index: an indec showing residential building costs in Toronto.<br>
<br>

In addition, a sixth parameter; total jobs in city of Toronto is also included.

### Based on data availability, monthly data for an 11 years window from January 2011 to December 2021 is considered in this analysis.

The structure of this report is as follow:<br>
<br>
1- Data<br>
2- Exploratory Data Analysis<br>
3- Forecasting Housing Prices<br>
4- Summary, recommendations and future work<br>


#Summary, recommendations and future work

## Summary:

An analysis is conducted to find the two most important parameters that affect housing prices in city Toronto. To this end, datasets from six different public sources were gathered and compiled to analyze the influence of following parametrs on housing prices:<br>
<br>
* Real income<br>
* The cost of mortgages<br>
* Construction and development costs<br>
* Land availability<br> 
* Location and housing stock supply and demand<br>
* Job market prosperity

Three types of analysis is performed:<br>
<br>
1- Correlation analysis<br>
2- Granger causality test<br>
3- Random forest feature importance<br>

Results of this analysis suggest that 'Average residential building construction cost' and 'land value' are the most important parameters affecting housing prices in Toronto.<br>

## Recommendation:

Based on the results of this analysis and recommendations from Ontario Housing Affordability Task Force report in 2020 (https://www.ontario.ca/page/housing-affordability-task-force-report) one policy change is suggested that influences both identified parameters in order to reduce housing prices in Toronto:<br>

**Give the province the authority to impose standards related to zoning, density and urban design and lessen the power that cities have over housing developments.** <br>
This way, province can repeal municipal policies that focus on preserving a neighbourhood's character and reduce land prices especially for expensive neighbourhoods.<br> 
In addition, one of the factors that influence construction costs is very long project approval times; province can legislate timelines for development approvals, and if the municipality misses the deadline, the project gets an automatic green light.<br>

## Future work:
- I would meet with subject matter experts to understand the problem/data better, and find other useful data categories.
- This is a simplified model, more detailed parameters such as type of buillding (house, condo, etc.), demographic information on wges (age, sex, ype of employment, etc.), breakdown of employements to NAICS Sector (finance, mining, health care and social assistance, etc.), etc. can be added.
- Search for additional parameters that might affect housing prices in Toronto.
- Hyperparameter tune the random forest model.
- Try other algorithms for forecasting housing prices such as RNNs and LSTMs.

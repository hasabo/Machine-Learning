With the increase in the number of crimes taking place in London, law enforcement agencies are trying their
best to understand the reason behind such actions. For this reason, the London Metropolitan Police Service
decides has released a new challenge: understand trends and patterns that will help predict any future
occurrences of criminal activities in the streets of London.
Analyses like these are useful for two equally important reasons. First, to help understand the reasons
behind the major crimes. Second, to predict where crimes may occur and therefore to prevent further
occurrences.
The London Metropolitan Police Service has available two main datasets, holding the following structure:
Crime data:
WardCode. Geographical unit of analysis. It is a code corresponding to an electoral London area.
WardName. Name of the corresponding electoral London area.
NESW. Whether the ward is located in the north, south, west, east part of London.
CST4070 - Applied Data Analytics - Tools,
Practical Big Data Handling, Cloud Distribution
Formative assessment
General information
nd
The challenge
Data
Borough. London Borough to which the ward corresponds to.
MajorCategory. Category (top level) of the crime (e.g., "Burglary", "Criminal Damage", "Drugs").
MinorCategory. Category (low level) of the crime (e.g., "Burglary In A Dwelling", "Burglary In Other
Buildings").
T_201004, ..., T_201801. A sequence of attributes denoting the number of crimes occurring in a given
year (first four digits of the attribute) and in a given month (last two digits of the attribute). As an
example, the attribute T_201004 corresponds to the year 2010 (first four digits) and to the month 04
(last two digits), which is April.
Census data:
WardCode. Geographical unit of analysis. It is a code corresponding to an electoral London area.
WardName. Name of the corresponding electoral London area.
AreaSqKm. Square kilometres associated with the corresponding ward.
lon, lat. Coordinates (longitude, latitude) associated with the centre of the ward.
IncomeScor. Proportion of the population experiencing deprivation relating to low income. The more
deprived is an area, the higher the score.
LivingEnSc. Quality of the local environment. The more deprived is an area, the higher the score.
NoEmployee. Number of people having an occupation.
ArtsEmploy. Number of people working in art.
GrenSpace. Percentage of green space associated with the ward.
PopDen. Population divided by the surface of the ward area.
BornUK. Total number of people who were born in the UK.
NotBornUK. Total number of people who were not born in the UK.
NoCTFtoH. Number of properties in council tax band F-H (the highest median house price)
NoDwelling. Number of properties in each ward.
NoFlats. Number of flats in each ward.
NoHouses. Number of houses in each ward.
NoOwndDwel. Number of owned properties in each ward.
MedHPrice. Median house price.
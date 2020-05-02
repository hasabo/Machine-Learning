Santander Cycles (formerly Barclays Cycle Hire) is a public bicycle hire scheme in London. The scheme's bicycles are popularly known as Boris Bikes, after then-Mayor of London, Boris Johnson. The operation of the scheme has been contracted by Transport for London (TfL). The recent success of the scheme has led to its expansion into many areas of London and its rapid growth has led to real challenges balancing bike sharing supply with bike sharing demand.
To provide a possible solution to this problem, bike sharing usage prediction is critical. To this purpose, the Transport for London (TfL), has released three dataset − named bike_journeys , bike_stations and London_census − whose structure is illustrated in the next section.
As part of the challenge, you need to define and implement a data science method able to predict the total number of bikes rented in each bike station with the temporal granularity of one hour time slot, so to help TfL to balance bike sharing supply with bike sharing demand.
Special attention must be paid to the interpretation of the final adopted model, to understand which factors are associated with an high/low demand of rented bikes in London, such as population composition from census data, weekends, peak hours, and so forth.
     
Data
Three dataset available, which have the following structure. bike_journeys data:
Journey_Duration: duration of the bike journey in seconds.
Journey_ID: the id of the journey.
End_Date: a numeric field indicating the day of the month when the journey terminated (e.g., 1, 2, ..., 30, 31).
End_Month: a numeric field indicating the month when the journey terminated (e.g., 1, 2, ..., 11, 12). End_Year: a numeric field indicating the year when the journey terminated (e.g., 2017).
End_Hour: a numeric field indicating the hour when the journey terminated (e.g., 1, 2, ..., 23, 24). End_Minute: a numeric field indicating the minute when the journey terminated (e.g., 1, 2, ..., 59, 60). EndStationID: the id of the station where the journey terminated.
Start_Date: a numeric field indicating the day of the month when the journey started (e.g., 1, 2, ..., 30, 31).
Start_Month: a numeric field indicating the month when the journey stated (e.g., 1, 2, ..., 11, 12). Start_Year: a numeric field indicating the year when the journey started (e.g., 2017).
Start_Hour: a numeric field indicating the hour when the journey started (e.g., 1, 2, ..., 23, 24). Start_Minute: a numeric field indicating the minute when the journey started (e.g., 1, 2, ..., 59, 60). StartStationID: the id of the station where the journey started.
bike_stations data:
Station_ID: the id of a bike station.
Capacity: a numeric value indicating the maximum capacity of bikes of the station.
Latitude: the latitude where the station is located.
Longitude: the longitude where the station is located.
Station_Name: a string indicating the name of the station (e.g., "River Street , Clerkenwell", "Phillimore Gardens, Kensington").
LondonCensus data:
WardCode: geographical unit of analysis for the census data. It is a code corresponding to an electoral London area.
WardName: name of the corresponding electoral London area.
Borough: London Borough to which the ward corresponds to.
NESW: whether the ward is located in the north, south, west, east part of London.
AreaSqKm: square kilometres associated with the corresponding ward.
lon, lat: coordinates (longitude, latitude) associated with the centre of the ward.
IncomeScor: proportion of the population experiencing deprivation relating to low income. The more deprived is an area, the higher the score.
LivingEnSc: quality of the local environment. The more deprived is an area, the higher the score. NoEmployee: number of people having an occupation.
GrenSpace: percentage of green space associated with the ward.
PopDen: population divided by the surface of the ward area.
BornUK: total number of people who were born in the UK.
NotBornUK: total number of people who were not born in the UK.
NoCTFtoH: number of properties in council tax band F-H (the highest median house price) NoDwelling: number of properties in each ward.
NoFlats: number of flats in each ward.
NoHouses: number of houses in each ward.
NoOwndDwel: number of owned properties in each ward.
MedHPrice: median house price.
                             

# CrimeIncidents_WashingonDCState

### Project Information 
Timeline for the crime incidents which has happened in the WashingtonDC State of United States of America in the Year 2018. (Final Output can be seen : [Here](jpg/WashingtonDC_CrimeIncidents_2018Timeline.gif))

### Data Sets : 
1. Crime Incident Data : Taken from [Data-World](https://data.world/dcopendata/38ba41dd74354563bce28a359b59324e-0)
2. Washington Grid Data : Taken from the [DC Goverment wesbite](https://opendata.dc.gov/datasets/washington-dc-boundary)


### CRS 
1. Data was parsed into the EPSG4326 format. More details about WGS1984 can be found [here](https://epsg.io/4326)
2. Both the data was asserted to have the same CRS format. 

### Data Processing
1. Crime Data had timestamp in object format, and had to be converted to DT object where the Month was extracted to group the data month wise. 
2. Esri shape file doesn't support datatime, and hence the datatime column had to be removed. 


magick convert -delay 60 -loop 0 CasesInJanuary.jpg CasesInFebruary.jpg CasesInMarch.jpg CasesInApril.jpg CasesInMay.jpg CasesInJune.jpg CasesInJuly.jpg CasesInAugust.jpg CasesInSeptember.jpg CasesInOctober.jpg CasesInNovember.jpg CasesInDecember.jpg WashingtonDC_CrimeIncidents_2018Timeline.gif

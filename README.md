# Seattle Municipal Solid Waste 2000-2019

This dataset was curated for Data Curation 1 (LIS 545), a course offered by the iSchool at the University of Washington as part of their MLIS program. It contains data [provided by Seattle Public Utilities](http://www.seattle.gov/Documents/Departments/SPU/Documents/Recycling_Rate_Report_2019.pdf) (SPU) about their Municipal Solid Waste program (MSW), including tonnage of MSW generated, disposed (sent to landfill), and recycled; recycling rate per year; population size of the city; and year-over-year (YOY) comparisons of these metrics. The data span 20 years, from 2000-2019.

The dataset consists of 3 CSV files, one for each MSW waste stream: Residential, Commercial, and Self-Haul. Year, Seattle's population, and the population's YOY change are duplicated across all 3 files to increase interpretability. If the dataset were instead structured as a relational database, there would be a separate table for population and all tables could be joined on the year.

This dataset is relevant to researchers who are interested in assessing the effectiveness of urban recycling initiatives in a large, growing city. Of particular note is Seattle’s ability to grow in population size by over 30% between 2000-2019 while maintaining a relatively stable amount of MSW generated over the same period.

## Naming Conventions
Filenames follow the convention:
```
seattle_msw_{stream}.csv
```
where `{stream}` denotes the waste stream the data refer to, which should be one of `commercial`, `residential`, or `selfhaul`.

## Data Dictionary

| **Variable** | **Variable Type** | **Measurement Unit** | **Allowed Values** | **Description** |
| --- | --- | --- | --- | --- |
| **year** | int | year | calendar years | the year for which the other variables in the same row apply |
| **msw\_generated** | int | tons | positive integers | total tons of Municipal Solid waste generated for the year |
| **msw\_disposed** | int | tons | positive integers | total tons of Municipal Solid waste disposed (sent to landfill) for the year |
| **msw\_recycled** | int | tons | positive integers | total tons of Municipal Solid waste recycled (including compost) for the year |
| **msw\_recycle\_rate** | float | percentage | positive floats | percentage of total Municipal Solid Waste generated that was diverted from landfills through recycling and composting |
| **seattle\_population** | int | number of people | positive integers | population count of Seattle for the year |
| **yoy\_msw\_generated** | float | percentage | floats | year-over-year percentage change in amount of Municipal Solid Waste generated |
| **yoy\_msw\_disposed** | float | percentage | floats | year-over-year percentage change in amount of Municipal Solid Waste disposed (sent to landfill) |
| **yoy\_msw\_recycled** | float | percentage | floats | year-over-year percentage change in amount of Municipal Solid Waste recycled (including compost) |
| **yoy\_recycle\_rate** | float | percentage | floats | year-over-year percentage change in total Municipal Solid Waste generated that was diverted from landfills through recycling and composting |
| **yoy\_population** | float | percentage | floats | year-over-year percentage change in Seattle population |

## Metadata
Schema Used: Project Open Data

| **Attribute** | **Value** |
| --- | --- |
| accessLevel | public |
| accrualPeriodicity | R/P1Y |
| fn | Brandon Aleson |
| hasEmail | [alesausk@uw.edu](mailto:alesausk@uw.edu) |
| describedBy | https://github.com/barlaensdoonn/seattle-municipal-solid-waste-2000-2019/blob/main/README.md |
| description | This dataset contains 20 years (2000-2019) of data for Seattle Public Utilities' Municipal Solid Waste program, including tons of waste generated, disposed, and recycled/composted for 3 waste streams: Residential, Commercial, and Self-Haul. The intended audience are researchers. |
| accessURL | https://github.com/barlaensdoonn/seattle-municipal-solid-waste-2000-2019 |
| downloadURL | https://github.com/barlaensdoonn/seattle-municipal-solid-waste-2000-2019/archive/main.zip |
| format | CSV |
| mediaType | CSV |
| issued | 2021-03-10 |
| keyword | &quot;recycling&quot;, &quot;compost&quot;, &quot;municipal solid waste&quot;, &quot;seattle&quot; |
| landingPage | https://github.com/barlaensdoonn/seattle-municipal-solid-waste-2000-2019 |
| language | en-us |
| modified | 2021-03-10 |
| publisher | Brandon Aleson |
| references | [http://www.seattle.gov/Documents/Departments/SPU/Documents/Recycling_Rate_Report_2019.pdf](http://www.seattle.gov/Documents/Departments/SPU/Documents/Recycling_Rate_Report_2019.pdf) |
| Rights | These data are freely available to the public for all use and reuse |
| temporal | 2000-2019 |
| theme | recycling, municipal solid waste |
| title | Seattle Municipal Solid Waste 2000-2019 |

## Rights

These data are freely available to the public for all use and reuse

## Contact
Brandon Aleson
alesausk@uw.edu

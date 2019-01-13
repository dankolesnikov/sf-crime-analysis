# UCSB Hacks Project
> Emerson Ye, Danil Kolesnikov

## Branches

* master - main branch with **stable** code
* danil - Dan's work
* emerson - Emerson's work

## SF Crime Data

### Insights
> What questions to be answered?

1. What districts have the highest number of violent crimes in SF?
   * define violent
   * heat map of violent crimes using Folium library
2. What district has the most number of violent crimes?
3. What days of the week has the most amount violent crimes in each district? Overall?

%%gcs read --object gs://ucsb_hacks_datasets/sf-crime-data-filtered.csv	--variable crime_data
df = pd.read_csv(StringIO(crime_data))


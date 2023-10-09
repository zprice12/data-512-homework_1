# Data 512 - Homework 1
## Project Goal
The goal of this project is to create informative time series graphs to investigate page requests for specific movie-related wikipedia articles.
## Licenses and Links
Source Data License -  
https://creativecommons.org/licenses/by/4.0/  
Wikimedia Foundation REST API Terms of Use -  
https://www.mediawiki.org/wiki/API:REST_API#Terms_and_conditions  
REST API Documentation -  
https://wikimedia.org/api/rest_v1/#/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end  
Pageviews API Documentation -  
https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews
## Data Files
### thank_the_academy.AUG.2023.csv
This data file includes the articles we wish to investigate in this project. It includes a name field with the name of the article and a url field with a url to each article.
### academy_monthly_mobile_201507-202309.json
This data file includes monthly mobile page requests for each article. It involves an article field with the name of the article, a timestamp field with year and month, and a views field that represents the total monthly views for each article.
### academy_monthly_desktop_201507-202309.json
This data file includes monthly desktop page requests for each article. It involves an article field with the name of the article, a timestamp field with year and month, and a views field that represents the total monthly views for each article.
### academy_monthly_cumulative_201507-202309.json
This data file includes monthly cumulative page requests for each article. It involves an article field with the name of the article, a timestamp field with year and month, and a views field that represents the total monthly views for each article.
## Special Considerations
A forward slash in article titles will cause and error with the urllib function in the API call. This can be fixed by setting safe=''.

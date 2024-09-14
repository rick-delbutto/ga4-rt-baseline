# ga4-rt-baseline
Analytics Pioneers Hackathon - GA4 real time "baseline" checker of hits

The main goal of the baseline checker is to have a system in place which is taking the real time data of Google Analytics API and check all events for a deviation after changes. As soon as a new version of the container is published, the Analytics expert would like to see if GA4 data is still being collected as expected. Therefore, we are trying to setup a "baseline" checker, to see if the different hits are working as expected within the thresholds of the deviation (~5%). 

### Google Analytis Reporting API
To get access to the Google Analytics Reporting API, a GCP project is required. After successful creation, add and enable the API to get access. It can be found under `APIs & Services > Enabled APIS & services`. 
Google Analytics Data API needs to be enabled. It is not automatically available within your project. 

### Create a GCP Service Account 
The service account will get the data from the API and will be added to the GA4 property with the necessary permissions. 

### Set GA4 permissions for the service account
The newly created service account will need to be added to GA4. 

### Get the data with Python
---

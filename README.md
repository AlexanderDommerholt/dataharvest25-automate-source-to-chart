# Dataharvest session: Using free tools to automate your data flows from source to chart

### What you will learn:

How to ...

* collect data from a url
* parse the data into the needed format using Python's `pandas` library
* use Python's [`datawrapper` library](https://datawrapper.readthedocs.io/en/latest/user-guide/api.html#datawrapper.Datawrapper.update_description) to create a chart
* set up the script to run automatically on [Github Actions](https://docs.github.com/en/actions/administering-github-actions/usage-limits-billing-and-administration#availability)


### Prerequesites for the session: 

*Basic coding or Python knowlegde is helpful but not required*

* required: Access to colab.google.com (if you already have a Google account that's available)
* required: [Datawrapper API token](https://academy.datawrapper.de/article/225-what-you-can-do-with-our-api-and-how-to-use-it)
* required: Github Account (if you want to set up the workflow to be automated)
* optional: [Distill Browser Plugin](https://distill.io/) (if you want to set up the workflow on click)


### Code & Data

**Code**: To follow along, you'll need to make yourself a copy of this jupyter notebook on Google colab.

**Data source**: For this session, we'll be working with the [UNHCR data on arrivals to Europe via land and sea](https://data.unhcr.org/en/situations/europe-sea-arrivals), more specifically: with the URLs provided on the page to the json data

* all arrivals (sea + land): "https://data.unhcr.org/population/get/timeseries?widget_id=588956&sv_id=100&population_group=4797,4798,5634&frequency=month&fromDate=2016-01-01"
* sea arrivals: "https://data.unhcr.org/population/get/timeseries?widget_id=588957&sv_id=100&population_group=4797,5634&frequency=month&fromDate=2016-01-01"
* land arrivals: "https://data.unhcr.org/population/get/timeseries?widget_id=588958&sv_id=100&population_group=4798&frequency=month&fromDate=2016-01-01"



cma_import_script
=================

Script showing usage of the [contentful-management](https://github.com/contentful/contentful-management.rb) gem which is a wrapper for the [Content Management API](https://www.contentful.com/developers/documentation/content-management-api/).

## Description
CMA import script is a showcase how you can play with the [contentful-management](https://github.com/contentful/contentful-management.rb) gem in order to load your data to the Contentful platform.
Script uses [Open Beer Database](http://openbeerdb.com/), which includes such domain models:
- Brewery
- Beer
- Category
- Style

Script loads only selected probe of items due to size of the data (time of execution).
You can change preselected set of breweries and beer styles by changing: BREWERIES_IDS and STYLE_IDS constants in the script.

## Installation
```
$ bundle install
```

## Data source setup
Download [openbeerdb_csv.zip](http://openbeerdb.com/data_files/openbeerdb_csv.zip) from [Open Beer Database](http://openbeerdb.com/) and unzip it into data directory.

## Usage
Note that you need to specify your access token and organization id in the script.rb file (ACCESS_TOKEN, ORGANIZATION_ID). 
Your access token can be found at [CMA - documentation](https://www.contentful.com/developers/documentation/content-management-api/#getting-started)

Script execution:

```
$ ruby script.rb
```



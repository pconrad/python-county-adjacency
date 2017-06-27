# python-county-adjacency
A simple Python library that wraps US County Adjacency data

By Phill Conrad

# What this library does

This library provides a Python wrapper around data from the file https://www2.census.gov/geo/docs/reference/county_adjacency.txt (a copy of which is cached in this repo), that allows a user to determine, for any US county, what counties are adjacent to that county (i.e. share a border with it.)

# Details

Counties are provided for:
* all 50 US States (accessed by their standard USPS two-letter state abbreviations)
* the District of Columbia ("DC"), treated as a single county equivalent for purposes of this dataset

Note that in Louisiana, the equivalent of a county is called a "parish". 

Counties are also provided for the following US territories.  A flag can be set to include or exclude these territories from the data, since including or excluding them may be approrpriate depending on the use case.  To keep the API simple, when they are included, they are treated as "states" for purposes of the API, even though their legal status is different from that of a US state.   Each of these has its own designator for what a "county equivalent" is called.

| Territory | Code | County Equivalent |
|-----------|----------------------|
|  Puerto Rico | PR | Municipio |
|  American Samoa | AS | Island or District (both appear in the data) |
|  Guam | GU| (treated as a single county)|
|  Puerto Rico | PR | Country Equivalent |


# Motiviation

Suppose you are accessing data by US county, for example, [this dataset](https://think.cs.vt.edu/corgis/json/food_access/food_access.html) from the United States Department of Agriculture's Economic Research Service.   That data set contains information about access to sources of healthy and affordable food (and is provided courtesy of the [Corgis project at Virginia Tech](https://think.cs.vt.edu/corgis/).

You might 




You might want to bring up data for your own county, and The file https://www2.census.gov/geo/docs/reference/county_adjacency.txt has data for US County adja

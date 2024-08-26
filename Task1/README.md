# Task 1

## Gather Data Using APIs

Our assignment is to get the number of job openings using the GitHub Jobs API for technologies like:

- Java
- Python
- MySQL
- C++
- C#

Since GitHub Jobs has now been deprecated we will be hosting our own JOBS_API backend on Flask to mimic the service. The data is populated from the following source: https://www.kaggle.com/promptcloud/jobs-on-naukricom under a **Public Domain license**.

> Note: We are using a modified subset of that dataset rather than the dataset from the original source.
> The original dataset is a CSV. We have converted the CSV to JSON as per the requirement of this project.

### Github Jobs Information

GitHub Jobs API allows anyone to query for the jobs based upon:

- Technology like Python, MySQL
- City like New York, Bangalore

Here are the technical details to access the API.

The GitHub Jobs API allows you to search, and view jobs with JSON over HTTP.

To get the JSON representation of any search result or job listing, append .json to the URL you’d use on the HTML GitHub Jobs site.

For example, the below URL will search for Python jobs near New York:

https://jobs.github.com/positions?description=python&location=new+york

To get the JSON representation of those jobs, just use positions.json:

https://jobs.github.com/positions.json?description=python&location=new+york

Pagination
The API also supports pagination. /positions.json, for example, will only return 50 positions at a time. You can paginate results by adding a page parameter to your queries.

Pagination starts by default at 0.

Examples
https://jobs.github.com/positions.json?description=ruby&page=1

https://jobs.github.com/positions.json?page=1&search=code

GET /positions.json
Search for jobs by term, location, full-time vs part-time, or any combination of the three. All parameters are optional.

Parameters
description — A search term, such as “ruby” or “java”. This parameter is aliased to search.
location — A city name, zip code, or other location search term.
lat — A specific latitude. If used, you must also send long and must not send location.
long — A specific longitude. If used, you must also send lat and must not send location.
full_time — If you want to limit results to full-time positions set this parameter to ‘true’.
Examples
https://jobs.github.com/positions.json?description=python&full_time=true&location=sf

https://jobs.github.com/positions.json?search=node

https://jobs.github.com/positions.json?lat=37.3229978&long=-122.0321823

GET /positions/ID.json
Retrieve the JSON representation of a single job posting.

Parameters
markdown — Set to ‘true’ to get the description and how_to_apply fields as Markdown.

Examples
https://jobs.github.com/positions/21516.json

https://jobs.github.com/positions/21516.json?markdown=true

## Gather Data Using Web Scraping

Gather Average Salary Information from this website: https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DA0321EN-SkillsNetwork/labs/datasets/Programming_Languages.html

The data we need to scrape is the name of the programming language and average annual salary.

- Extract information from a given web site
- Write the scraped data into a csv file.

## Exploring Data

Goals:

- Load the dataset that will be used throughout the capstone project.
- Explore the dataset.
- Get familier with the data types.

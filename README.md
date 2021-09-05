# Web-Scraping-Multiple-Pages

## Web Scraping Multiple Pages of the IMDB movies

>- This repository is an extension of my previous repository where we were scraping data from a single page [Web scraping](https://github.com/wakibia/Web_scraping)
>- The reason for choosing the IMDB repository its because the way web pages are changing is quite complicated.
>- We seek to scrape the data for the movies generated from First January to December 31st 2020
>- The link to the data is [IMDB 2020](https://www.imdb.com/search/title/?title_type=feature&release_date=2020-01-01,2020-12-31&count=100&ref_=adv_prv)

## Web Scraping Procedure

>- The scraping procedure is similar to the one discussed at [Web scraping](https://github.com/wakibia/Web_scraping)
>- The additional steps required is only creating a function that will help in iterating the process from one page to the other
>- To achieve iteration from one page to another we will use r`purrr` package which has a set of different map function

## Variables to be SCraped

>- Since this is for pedagogical purposes we are going to scrape only 3 pages but the procedure is the same. This is because the higher the number of pages to be scraped the longer it will take

The following are the variables that will be scraped along with their descriptions:

| Variable | Description |
| ------  | -------- |
| Rank | The rank of the film from 1 to 100 on the list of 100 most popular feature films released in 2016 |
| Title | The title of the feature film |
| Description | The description of the feature film |
| Runtime | The duration of the feature film in minutes |
| Genre:| The genre of the feature film |
| Rating | The IMDb rating of the feature film |
| Votes | Votes cast in favor of the feature film |
| Director | The main director of the feature film. Note, in case of multiple directors, I’ll take only the first |
| Actor | The main actor in the feature film. Note, in case of multiple actors, I’ll take only the first |


After scraping the data, the data frame will be exported to a csv file which can later be retrieved from a local environment

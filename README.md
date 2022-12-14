# NCAA-Basketball-Games-Predictor

This repo contains models aimed at predicting regular season outcomes of NCAA Men's Division I Basketball.

## Acknowledgements

I want to acknowledge Sports-Reference (https://www.sports-reference.com/cbb/) and Bart Torvik (https://barttorvik.com/#) as the data for NCAA Basketball teams was pulled from there.

## The Datascraper

The file game_log_datascraper.py contains the method for getting information to train the models on. We are primarily interested in scraping individual game logs of all D1 schools. The scraper pulls data from Sports-Reference, so if the scraper is applied to another website, it might not work. Moreover, the URL that the scraper pulls data from must be changed each season, as it will need to scrape data from the newer season of college basketball. The scraper will output a CSV file containing the game logs of all D1 schools. To use the scraper, simply type: 

``` python src/game_log_datascraper.py ```

The file school_stats_datascaper.py contains the method for getting data for overall school averages in a given year. The scraper pulls data from Sports-Reference, so if the scraper is applied to another website, it might not work. Moreover, the URL that the scraper pulls data from must be changed each season, as it will need to scrape data from the newer season of college basketball. The output again is a CSV file containing the school stats of D1 schools. To use, type:

``` python src/school_stats_datascraper.py ```

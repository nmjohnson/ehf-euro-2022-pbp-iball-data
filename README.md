# ehf-euro-2022-pbp-iball-data
A repository for EHF EURO '22 play-by-play with iBall data

## Synopsis

With the 3rd version of the live ticker data for EHF events, tracking data has been made available for the men's european championship in 2022 and presumably for all EHF going forward. This repository contains the raw live ticker json's which provide play-by-play, metadata, and aggregate tracking data. Additionally one csv file which provides iBall shot tracking data (shooter location, shot on goal location, speed, distance, etc) for all matches. While you can access shooter location and shot on goal location from within the liveticker page. In addition to EURO championship matches this also includes all qualificaiton matches going back to 2020. 

![Example of some iBall data](iball_preview.JPG)

## Accessing the iBall data

To access the full set of iBall data, one must click on an individual on the live ticker page and then click on the "player shot details" button. This will bring a visualization up of where the shooter was for each attempt, where the ball location was on the goal, and whether or not a goal was scored. Clicking on the circle for each shot will also reveal the speed (in km/h), the distance (in m) and the time at which the attempt occurred. While one can click through every player in every game, and click on each shot to reveal all of this information, I figured it was much easier to create a script to scrape all of this information and put it in one spot, which is the [shotdata.csv](https://github.com/nmjohnson/ehf-euro-2022-pbp-iball-data/blob/main/data/shotdata.csv) file in this repository. 

## Final thoughts

There is no warranty or data quality guarantee with this files in this repository. Since the source is a sensor based tracking system I expect the measurements to be quite precise, but I can't guarantee that that raw data made it perfectly through all the way to the live ticker page. If you notice any corrections, please let me know and file an issue in the repo and I can update the files as needed.

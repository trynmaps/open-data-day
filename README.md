# [OpenTransit](http://opentransit.city/) x [Open Data Day 2019](https://www.eventbrite.com/e/code-for-san-francisco-open-data-day-2019-tickets-56291530483)

Welcome to Open Data Day 2019! Today, we're going to give you a full day's worth of raw
data about the buses in San Francisco -- you'll know where every bus in the city was
every 15 seconds on October 15, 2018. It's 230 MB of raw, unprocessed open data.

Your challenge is to make something useful for San Franciscans with it.

To give you a taste of how the open data analysis process goes, we'll be giving snapshots
of our data at 3 stages in the analysis process: totally raw, processed, then improved.
Choose a stage and try to improve upon our work!

At the end of the day, we encourage you to make a pull request with your code,
and we'll incorporate the best code into the [data visualization prototype we're building](https://github.com/trynmaps/metrics-mvp).

# The challenges

We have a separate challenge for each stage. We'll give you the data for that stage
and the code we've written so far to get the data to the next stage.

Can you come up with better algorithms and visualizations than us?

## Challenge 1: Calculating bus stops

Our raw data -- the location of each bus at each point in time -- isn't terribly
useful by itself. Our first task was to turn this raw data into 
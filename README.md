# [OpenTransit](http://opentransit.city/) x [Open Data Day 2019](https://www.eventbrite.com/e/code-for-san-francisco-open-data-day-2019-tickets-56291530483)

Welcome to Open Data Day 2019! Today, we're going to give you a full day's worth of raw
data about the buses in San Francisco -- you'll know where every bus in the city was
every 15 seconds on October 15, 2018. It's 230 MB of raw, unprocessed open data.

Your challenge is to make something useful for San Franciscans with it.

To give you a taste of how the open data analysis process goes, we'll be giving snapshots
of our data at 3 stages in the analysis process: totally raw, somewhat cleaned, then processed.
Choose a stage and try to improve upon our work!

At the end of the day, we encourage you to make a pull request with your code,
and we'll incorporate the best code into the [data visualization prototype we're building](https://github.com/trynmaps/metrics-mvp).

# The challenges

We have a separate challenge for each stage. We'll give you the data for that stage
and the code we've written so far to get the data to the next stage.

Can you come up with better algorithms and visualizations than us?

## Challenge 1: Interpolation

The big problem with our raw data is that it's pretty coarse: we can only get
each bus's location every 15 seconds. To enable smoother tracking, mapping,
and predicting, we want to interpolate where buses were between those 15-second
intervals -- say, every 5 seconds.

To help you simulate this, we'll give you a version of our raw data file
that only gathers data at 30-second intervals and challenge you to make an
algorithm that interpolates the bus's location every 15 seconds. Then you can
compare your results to our *actual* data file, which tracks buses' real
locations every 15 seconds. If your algorithm predicts the 15-second locations well,
we'll use it on our actual data file to compute where the bus was every 5 seconds.

## Challenge 2: Bus Stop Computation

Even when cleaned, our raw data -- the location of each bus at each point in time
-- isn't terribly useful by itself. Our next task was to turn this raw data into
a dataset of when each bus reached each stop (e.g. when did bus #123 on route 14
reach 9th & Market?)

We've developed a processing algorithm to calculate the bus stops, but we challenge
you to do better. You'll have access to the 230 MB of raw data and our algorithm.
Can you find a better way to compute stops?

> Note: The 230 MB file takes a while to process. Check out the light file
> we've included instead for a subset of the data that is smaller and faster
> to process.

## Challenge 3: Metrics & Visualization

Our final challenge is to turn our processed data into useful metrics and
visualizations for San Franciscans.

So far, we've started computing and graphing wait time and travel time
for each line, brokend down by day of week and time of day. Can you find
other useful metrics and visualize it in interesting ways -- perhaps
drawing in geographic or economic data, or making it interactive?

# Getting Started

Fork this repository and choose the folder that corresponds to the challenge you want
to tackle. Each folder will contain the full 230 MB dataset, a light version that
includes a subset of the data, and a Jupyter notebook with our reference implementation
of the code.

You can create your own 
# [OpenTransit](http://opentransit.city/) x [Open Data Day 2019](https://www.eventbrite.com/e/code-for-san-francisco-open-data-day-2019-tickets-56291530483)

Welcome to Open Data Day 2019!

Today, we're going to give you raw and processed GPS data for Muni buses
in San Francisco.

Your challenge is to clean, analyze, and/or visualize that data and build
something useful for San Franciscans.

# The challenges

We have three challenges for you today, each one very similar to a challenge
our team of coders and analysts has had to tackle. For each, we'll give you
data to work with and sample code. Your job is to build something great
with the data.

At the end of the day, we encourage you to make a pull request with your code,
and we'll incorporate the best code into the [data visualization prototype we're building](https://github.com/trynmaps/metrics-mvp).

# Challenge 1: Processing

We've gathered raw data on where every Muni bus has been every 15 seconds for
over a year. Our first challenge was to convert this raw data into "arrival
times" -- so we could know when each bus reached each stop. Only then
could we start making interesting analyses and visualizations.

In this challenge, we'll give you a subset of our raw GPS data (we gather 230 MB
of data a day, so for simplicity's sake we're only giving you a few routes'
data). We'll also give you an example of our algorithm, which we call the "eclipses"
algorithm, that we use to calculate arrival times.

Your job is to make a better version of our arrival-time algorithm than the
"eclipses" algorithm.

To get started with this challenge, check out the [1-processing](1-processing) folder.

# Challenge 2: Analysis

Once we had computed the arrival times, we needed to start analyzing the
processed data to extract useful transit metrics.

In this challenge, we'll give you a sample of our pre-processed data, which shows
when each bus reached each stop (e.g. bus #123 on route #1 reached stop #456
at 3:45pm). The metrics we've calculated so far include average waiting time
at a given stop and average transit time between two stops.

Can you think up some more interesting metrics or find some interesting
patterns? Some questions you could try answering:

- At which time of the day are buses the latest?
- At which time of the day are buses the slowest?
- On which days of the week are buses faster or slower than average?
- When does there seem to be the most traffic?
- Did the bus ever take a detour or miss a stop?

To get started with this challenge, check out the [2-analysis](2-analysis) folder.

# Challenge 3: Visualization

The final challenge is to turn our data and metrics
and present them in a useful, informative way.

We'll give you the raw GPS data and our processed arrival time
data, as well as a sample Jupyter notebook with some demo
visualizations.

What's the coolest and most interesting visualization you can
make? For an added challenge, try adding in geographic, traffic,
or economic data, which you might be able to get from other
open data portals.

To get started with this challenge, check out the [3-visualization](3-visualization) folder.

## Challenge 3: Metrics & Visualization

Our final challenge is to turn our processed data into useful metrics and
visualizations for San Franciscans.

So far, we've started computing and graphing wait time and travel time
for each line, brokend down by day of week and time of day. Can you find
other useful metrics and visualize it in interesting ways -- perhaps
drawing in geographic or economic data, or making it interactive?

[Check out this folder](/visualization) to get started.

# Getting Started

Fork this repository and choose the folder that corresponds to the challenge you want
to tackle. Each folder will contain the full 230 MB dataset, a light version that
includes a subset of the data, and a Jupyter notebook with our reference implementation
of the code.

We suggest installing [Anaconda](https://www.anaconda.com/distribution/) to get iPython
on your machine.

Then clone this repository and `cd` into it. Then run `jupyter notebook` in your terminal
to browse, run, and play with our interactive Python notebooks.

# Submission

If you want our project to use your code, just make a pull request of your fork! We'll
review it and incorporate the best submissions into our
[prototype](https://github.com/trynmaps/metrics-mvp).

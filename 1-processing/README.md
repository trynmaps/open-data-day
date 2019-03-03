# Challenge 1: Bus Stop Computation

## Background/Motivation

The bulk of the raw data that we have access to is geolocation data - in particular, the location of every bus in the city, obtained every 15 seconds. In many cases, the first step to analyzing this data will be to find when a bus arrives at a stop along its route. This process often involves computing the distance between a given bus stop and thousands of points of geolocation data, and can therefore be very computationally intensive. Developing a fast, accurate algorithm for finding all of the bus arrival times from a set of raw geolocation data is critical - for instance, we would need this data if we wanted to know how long someone would expect to wait for a bus to arrive at a particular stop, or the average time it takes for buses to go from one stop to another.

## Challenge

We've developed an algorithm to approximate bus arrival times from the raw geolocation data. But it can take prohibitively long to run on large sets of data, i.e. geolocation data collected from many routes, over a long period of time. Can you develop a faster algorithm?

## Running the Example Notebook

The `sample_routes_data_pst_15s.json` file that the example notebook loads is zipped up in `sample_routes_data_pst_15s.rar`, so you'll have to extract it before running the notebook.
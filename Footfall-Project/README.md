# Updated Python File

Update -

1. First, we took lat-lon coordinates from the STOPS data , which contains lat-lon coords for all stops available in West Bengal area.

2. Now, we use the ROUTES data, the data that has all the bus routes data, route name, startstop and endstop

3. And finally, because ROUTES data did not have lat-lon coordinates, we tried to get the lat-lons of the start and end stops of a particular route from the STOPS data as it does have coords.

4. We plotted these stops for routes and the original stops.

5. Now, we took the  data for a single vehicle, running on a particular route , 218:DN , we have the coords of it's end and start points from the STOPS dataframe. 

6. Based on the movement of the vehicle for a single day , (MONDAY) , we try to plot its movemment.

# ISSUES - 

1.Not all stops in the ROUTES df are available in the STOPS df

2.Plotting bus data fro a single day, isn't giving any meaningful outocme , plot style can be changed, and there is no way to use  data for 7 days, as times are different so we cannot link movement of all days with a particular time of  day to average speed at that location.

3.We may use grouping of lat-lon coords to find the average speed betwween those locations for 7 days to defone a metric.

4. A proper shape file that gives roads of kolkata, isnt available for proper  plotting of data.


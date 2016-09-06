# Reproducible Research: Peer Assessment 1


## Loading and preprocessing the data

```r
activity_data <- read.csv("activity.csv") 
date <- as.Date(activity_data$date)
activity_data$date <- date
```

## What is mean total number of steps taken per day?

```r
mean_total = sum(activity_data$steps, na.rm = TRUE) / (nrow(table(activity_data$date)))
```


## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?

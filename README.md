#  AirBnb in Seattle

## Project Description

### Background on Data

Our group will be working with the **[AirBnb data](http://insideairbnb.com/get-the-data.html) collected on Seattle** as provided by **[InsideAirBnb](http://insideairbnb.com/about.html)**. InsideAirBnb is *“an independent, non-commercial set of tools and data that allows you to explore how Airbnb is really being used in cities around the world.”*

### Target Audience

Our target audiences are *tourists* and *visitors* in Seattle who use Airbnb to plan their stay. Because a wide variety of people are likely to visit Seattle, we are focusing on the demographic of people who prefer to select the most cost effective choice, such as younger adults.

The target audience would most benefit from learning about **cost effective options** to optimize the quality of their stay. Because **location** is one of the most important factors in selecting an Airbnb, our questions focus on exploring the *effects of location on price, availability, amenities and housing options*. By choosing location as an independent variable, our target audience can learn more about their options in Seattle based on where they want to stay. Analyzing the above variables would give us further insight into both AirBnb guests and the hosts.


### Specific Questions
* How does the location and the time of year affect the availability and pricing of AirBnb options?
* How does the pricing of AirBnb options affect available amenities?
* Which locations of Seattle AirBnb listings get the most positive reviews and which the most negative?
* What kind of features and amenities are the most commonly available in Seattle?

## Technical Description

### Reading in Data

We are using datasets provided by [InsideAirBnb](http://insideairbnb.com/get-the-data.html), specific to Seattle. InsideAirBnb provides several different useful datasets, all in `.csv` file format. Because the data is in a `.csv` file, we can use built in R functions to read in the file to a `dataframe` to analyze (i.e. `read.csv()`). The main dataset we are focusing on is the `listings.csv` summary dataset.

### Types of Data-Wrangling

The main summary listings dataset contains information regarding listing name, information regarding the hosts, information regarding the available AirBnb, as well as reviews and geographical data (i.e. latitude, longitude). There are many columns in the extensive and summary listings datasets that we will most likely not consider, such as columns like “cancelation”, which is a characteristic describing their cancellation policies, or “notes” which is a literal note left by the landlord. Therefore, `filtering` columns with `dplyr`, and parsing other string based column data (like the offered amenities for a listing) are steps that need to be taken to clean our data.

### Library Used in Project

* `library(“tidyverse”)` - includes `dplyr` and `ggplot2` among others
* `library(“leaflet”)` - interactive mapping

### Challenges

- One major challenge we anticipate is understanding the syntax and functions necessary to use shiny and our interactive mapping together in a cohesive graphical user interface.
- A second major challenge we anticipate is distributing tasks and working as a team remotely over GitHub, because there can be issues with communication, even workloads for everyone, and working towards a common goal.

## Links
Explore this report on the complete report and visualizations on [Shiny App](https://jasnel.shinyapps.io/seattle-airbnbs-visualization/).

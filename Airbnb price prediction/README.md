# Airbnb accommodation price prediction

Since 2008, guests and hosts have used Airbnb to expand on travelling possibilities and present more unique, personalized way of experiencing the world. This public dataset is a part of Airbnb describing the listing activity and metrics in NYC, NY for 2019.

![Hotel](https://github.com/Ranjini-G/INSAID-Assignment/blob/master/Images/Hotel.png "Hotel")

This data file includes 48895 samples and 16 metrics to find out more about hosts, geographical availability, necessary metrics to make predictions and draw conclusions.

| Column Name                      | Description                                           |
| -------------                    | -------------                                         |
| id                               | listing ID                                            |
| name                             | name of the listing                                   |
| host_id                          | host ID                                               |
| host_name                        | name of the host                                      |  
| neighbourhood_group              | location                                              |
| neighbourhood                    | area                                                  |
| latitudelatitude                 | coordinates                                           |
| longitudelongitude               | coordinates                                           |
| room_type                        | listing space type                                    |
| price                            | price in dollars                                      |
| minimum_nights                   | amount of nights minimum                              |
| number_of_reviews                | number of reviews                                     |
| last_review                      | latest review                                         |
| reviews_per_month                | number of reviews per month                           |
| calculated_host_listings_count   | amount of listing per host                            |
| availability_365                 | number of days when listing is available for booking  |

The goal is to predict the price of the accommodations. The analysis will also help understanding the busy neighbourhood and the need for accommodations, which will increase the listing in turn the revenue. Using Random Forest Regresser model for the predictions.

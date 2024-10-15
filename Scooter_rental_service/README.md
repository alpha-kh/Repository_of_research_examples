# Research of scooter rental service

**Project Description**

There is data on some users from several cities of the scooter rental service, as well as on their trips.

To travel around the city, users of the service use a mobile application.

The service can be used:
- without a subscription:
no subscription fee;
the cost of one minute of travel is 8 rubles.;
start-up fee (start of the trip) is 50 rubles;
- with an Ultra subscription:
subscription fee is 199 rubles per month;
the cost of one minute of travel is 6 rubles;
start-up fee is free.

To identify business growth points, it is necessary to analyze and compare data on users with and without a subscription, as well as test the following hypotheses:

- users with a subscription spend more time on trips;
- the average distance that users with a subscription travel in one trip does not exceed 3130 meters;
- monthly revenue from users with a subscription is higher by month than revenue from users without a subscription.

**Data Description**

The core data contains information about users, their trips and subscriptions.

Users — `users_go.csv`

* `user_id` - unique user identifier
* `name` - user name
* `age` - age
* `city` - city
* `subscription_type` - subscription type (free, ultra)

Rides — `rides_go.csv`

* `user_id` - unique user identifier
* `distance` - distance the user has traveled in the current session (in meters)
* `duration` - session duration (in minutes) — time from the moment the user clicked the "Start ride" button until the moment he clicked the "End ride" button
* `date` - date of the ride

Subscriptions — `subscriptions_go.csv`

* `subscription_type` - subscription type
* `minute_price` - cost of one minute of the ride for this subscription
* `start_ride_price` - cost of starting the ride
* `subscription_fee` - cost of the monthly payment

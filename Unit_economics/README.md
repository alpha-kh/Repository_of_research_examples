# Entertainment App data research

#### Project Description

There is data from an entertainment app about users attracted from May 1 to October 27, 2019: visits, purchases and advertising expenses.

*Goal:* identify the causes of losses and help the company get into the black.

*Task* analyze:
* where users come from and what devices they use,
* how much it costs to attract users from various advertising channels;
* how much money each client brings,
* when the costs of attracting a client pay off,
* what factors hinder customer acquisition.

#### Data Description

`visits_info_short.csv` - server log with information about site visits:

* `User Id` - unique user identifier,
* `Region` - user country,
* `Device` - user device type,
* `Channel` - referral source identifier,
* `Session Start` - session start date and time,
* `Session End` - session end date and time.

`orders_info_short.csv` - order information:

* `User Id` - unique user identifier,
* `Event Dt` - purchase date and time,
* `Revenue` - order amount.

`costs_info_short.csv` - advertising expense information:

* `dt` - advertising campaign date,
* `Channel` - advertising source identifier,
* `costs` - expenses for this campaign.

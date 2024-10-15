# Analysis of A/A/B test results for a startup (foodtech)

#### Project Description

There is data on user sessions of a mobile app of a startup that sells food products. The designers wanted to change the fonts in the entire app, and the managers believe that users will find it unusual. The decision will be made based on the results of the A/A/B test. Users were divided into 3 groups: 2 control groups with old fonts and one experimental group with new ones.

Goal: to find out which font is more effective by studying the behavior of app users and comparing the results of the A/A/B experiment

Tasks:

- get acquainted with the data and prepare it for analysis
- study the sales funnel, find out:
    - how users reach the purchase
    - how many users reach the purchase
- at what steps do users "get stuck" before they reach the purchase
- study the results of the A/A/B experiment and find out which font is better.

#### Data Description

In the `dataset.csv` file, each record is a user action or event.

- `EventName` is the name of the event;
- `DeviceIDHash` is the unique user identifier;
- `EventTimestamp` is the time of the event;
- `ExpId` is the experiment number: 246 and 247 are the control groups, and 248 is the experimental group.

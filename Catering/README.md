# Moscow catering

#### Project Description
The goal of the investors is to open a coffee shop in Moscow that is as cool and affordable as Central Perk. Investors are not embarrassed by the competition in this area, despite the fact that there are already enough coffee shops in big cities.

*Project Goal*: research the Moscow catering market, to give investors recommendations on opening a coffee shop based on the analysis results

*Tasks*:
- to familiarize yourself with the data;
- to study the data for anomalies, omissions, to eliminate them if possible, to bring the data into a form convenient for analysis;
- to analyze the data by quantity, ratings, categories and location of objects;
- to analyze the data separately for coffee shops and to give recommendations.

#### Data Description

There is a dataset with Moscow catering establishments for the summer of 2022. The information may have been added by users or found in publicly available sources. It is for reference only.

File `moscow_places.csv`:
- `name` — name of the establishment;
- `address` — address of the establishment;
- `category` — category of the establishment, for example, "cafe", "pizzeria" or "coffee shop";
- `hours` — information about the days and hours of operation;
- `lat` — latitude of the geographical point where the establishment is located;
- `lng` — longitude of the geographical point where the establishment is located;
- `rating` — rating of the establishment based on user ratings in Yandex Maps (the highest rating is 5.0);
- `price` — price category in the establishment, for example, "average", "below average", "above average", and so on;
- `avg_bill` — a string that stores the average order cost as a range, for example:
    - "Average bill: 1000–1500 ₽";
    - "Price of a cup of cappuccino: 130–220 ₽";
    - "Price of a glass of beer: 400–600 ₽" and so on;
- `middle_avg_bill` — a number with an estimate of the average bill, which is specified only for values ​​from the `avg_bill` column that begin with the "Average bill" substring:
    - If a row specifies a price range of two values, the column will contain the median of these two values.
    - If a row specifies a single number — a price without a range — this number will be entered into the column.
    - If there is no value or it does not begin with the "Average bill" substring, nothing will be entered into the column.
- `middle_coffee_cup` — a number with the price of one cup of cappuccino, which is specified only for values ​​from the `avg_bill` column that begin with the substring "Price of one cup of cappuccino":
    - If a row contains a price range of two values, the column will contain the median of these two values.
    - If a row contains one number - a price without a range, then this number will be entered into the column.
    - If there is no value or it does not begin with the substring "Price of one cup of cappuccino", then nothing will be entered into the column.
- `chain` — a number expressed as 0 or 1, which indicates whether the establishment is a chain (for small chains there may be errors):
    - 0 — the establishment is not a chain
    - 1 — the establishment is a chain
- `district` — the administrative district in which the establishment is located, for example, the Central Administrative District;
- `seats` — the number of seats.

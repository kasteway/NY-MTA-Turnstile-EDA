# The Breathe And Release Yogis For Employees



## Description: 

2020 was an unprecedented year filled with challenges. [Gallup’s latest state of the global workplace reports](https://www.gallup.com/workplace/349484/state-of-the-global-workplace.aspx) substantial increases in daily workplace stress and worry. Many of these symptoms were due to the self-isolation individuals faced when global borders closed and employers started remote-work.

According to the [National Institutes of Health](https://www.nccih.nih.gov/health/providers/digest/yoga-for-health-science), scientific evidence shows that yoga supports in stress management, mental health and well-being. Science has proven some of these benefits and The Breathe To Release yogis see a great opportunity to help the lives of employees in NY by offering free yoga and meditation sessions. 

The Breathe To Release are a group of highly motivated yogis with the goal of bringing awareness to the benefits of yoga and helping people achieve their potential. They have requested for an exploratory data analysis to be performed using subway station data to find out:
1. Which subway locations would be the best place to open a yoga studio?
      - Where are we likely to find employees on their way to work or home?	    
2. What time of the day should we offer the sessions with the main goal of attracting stressed employees?
      - Within the weekdays, which hours have the most traffic?


## Data: 

Data is provided by New York City Metropolitan Transportation Authority of the daily entries and exits of people using all the subway stations in the city by turnstile. The date range will be from August, 2021 to November, 2021.

The data from New York City is available at [MTA Turnstile Data](http://web.mta.info/developers/turnstile.html)


### Data Detail:

| Field Name | Description                                                                     |
|------------|---------------------------------------------------------------------------------|
| C/A        | Control Area                                                                    |
| UNIT       | Remote Unit for a station                                                       |
| SCP        | Subunit Channel Position represents an specific address for a device            |
| STATION    | Represents the station name the device is located at                            |
| LINENAME   | Represents all train lines that can be boarded at this station                  |
| DIVISION   | Represents the Line originally the station belonged to BMT, IRT, or IND         |
| DATE       | Represents the date (MM-DD-YY)                                                  |
| TIME       | Represents the time (hh:mm:ss) for a scheduled audit event                      |
| DESC       | Represent the "REGULAR" scheduled audit event                                   |
| ENTRIES    | The cumulative entry register value for a device                                |
| EXITS      | The cumulative exit register value for a device                                 |




## Tools:

  - SQLite3, DBbrowser and SQLAlchemy will be used to create a database

  - Python packages such as Numpy, Pandas and other packages for EDA 

  - Matplotlib, Seaborn to perform visualizations

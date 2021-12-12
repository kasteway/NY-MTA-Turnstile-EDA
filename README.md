# NY-MTA-Turnstile-EDA


# Description

The year 2020 was filled with unprecedented challenges. COVID-19’s impact has been immeasurable and continues to cause distributions to the lives of so many people. Gallup’s latest state of the global workplace reports substantial increases in daily workplace stress, worry and sadness reported by employees. Many of these symptoms were due to the self-isolation individuals faced when global borders closed and employers started remote-work.

According to the National Institutes of Health, scientific evidence shows that yoga supports in stress management, mental health and well-being. With many benefits of yoga scientifically proven, The Breathe To Release yogis see a great opportunity to help the lives of employees in NY by offering free yoga sessions for employees working in the city of New York to increase the quality of their lives. 

The Breathe To Release are a group of highly motivated yogis with the goal of bringing awareness to the benefits of yoga and helping people achieve their potential. They have requested for an exploratory data analysis to be performed using subway station data to find out:
1. Which subway locations would be the best place to open a yoga studio?
Where are we likely to find employees on their way to work or home?		
2. What time should the sessions be offered with the intention of attracting employees?


# Data
Data is provided by New York City Metropolitan Transportation Authority of the daily entries and exits of people using all the subway stations in the city by turnstile. The date range will be from August, 2021 to November, 2021.
I will try to add additional data such as the MTA station location using zip code or latitude and longitude to focus on different parts of the city. After the weekdays and hours have been analyzed, I would like to filter based on different parts of the city. 

The accessible data about the patterns of transit traffic in New York City is available[MTA Turnstile Data](http://web.mta.info/developers/turnstile.html) 



## Data Detail:

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
| DESC       | Represent the "REGULAR" scheduled audit event    |
| ENTRIES    | The cumulative entry register value for a device                                |
| EXITS      | The cumulative exit register value for a device                                 |


# Tools

SQLite, DBbrowser and SQLAlchemy will be used to create a database and use Python packages such as Pandas, Matplotlib, Seaborn to perform exploratory data analysis with visualization. 

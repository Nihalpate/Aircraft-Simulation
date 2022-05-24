# Introduction:
Everyday millions of people around the world uses commercial airliner travelling between one place to another, as a result, thousands of aircrafts are getting takeoff and land every minutes. To ensure smooth operation of all those aircrafts flying between one city to other we need to have most reliable schedule of takeoff timing and landing timing. Take off timing is obvious, but choosing landing timing for schedule is very critical, because we need to consider all the possible scenarios like, Early / Late departure, Taxi Timing at each airport, and In-air Timing (the time in-between Take-off and Landing), that is where Monte Carlo Simulation is very helpful.

# Procedure 
## Data Collection 
Data is crucial for creating any simulation. The data will provide detail information about the process or operation that we want to simulate. Here, in case of routine commercial airliner, we need several data around the fight like, Gate-departure at origin airport, Taxi time at origin airport, take off time, landing time, and Gate arrival at destination etc. these are all the time steps that are dependent on random events like, Departure Delays (+ for Delayed flight, - for Early flight and 0 for on time). The real data will give information on all the random variable included in the whole flight-duration. The "flightaware.com" is a good source of data related to commercial aviation. The row data that we collected is presented in the “Row Data.xlsx” file. 

## Data Prepration
Data Preparation is very important/tricky task especially it becomes hard when you are dealing with time arithmetic and your row data is in the “Text” format. In this simulation I have performed time arithmetic in Excel to derive different time duration. Most challenging task is to convert text date/time into actual date/time for deriving time duration. The data processing can be seen in the Excel sheet that is available in the repository as “Processed Data.xlsx”. 

### Noteble Excel Functions
MID() : use for selecting spacific text from text data in the EXCEL CELL.

TIME(): used to convert text into time data so, EXCEL can perform time calculaiton.

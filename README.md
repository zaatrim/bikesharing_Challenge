# ** NYC CitiBike Ride Sharing Analysis



## *Project Overview*
In this Analysis I will help Kate to perform an Analysis for CitiBike Sharing in City—Des Moines. for this analysis I will use New York Citi Bike data that has been released to the public for your analysis. for conducting this analysis I will use Pandas Library to perform the ETL process on the Data.  and Then I will Use Tableau to Run the analysis and present the outcome through the Tableau Story module.
    
                  
## *Analysis & Results*
### Analysis
1st step of the analysis, I need to use Pandas to Change Trip Duration to a Datetime Format. 

            import pandas as pd
            # 1. Create a DataFrame for the 201908-citibike-tripdata data. 

            # File to Load (Remember to change the path if needed.)
            citibike_data_to_load = "Resources/201908-citibike-tripdata.csv"

            # Read the 201908-citibike-tripdata data and store into a Pandas DataFrame
            citibike_tripdata_data_df = pd.read_csv(citibike_data_to_load)
            # Check top 10 Raws.
            citibike_tripdata_data_df.head(10)

            # 3. Convert the 'tripduration' column to datetime datatype.

            citibike_tripdata_data_df['tripduration'] = pd.to_datetime(citibike_tripdata_data_df['tripduration'], unit = 's')

            citibike_tripdata_data_df.head(10)
            # 4. Check the datatypes of your columns. 
            citibike_tripdata_data_df.dtypes

Next steps I will Import the transformed Data to Tableau and start using Tableau to build the following analysis:


1) Number of bikes checked out by duration for all users, filtered by the hour.
2) Number of bikes that are checked out by duration for each gender by the hour.
3) A heatmap showing the number of bike trips for each hour of each day of the week.
4) A heatmap showing the number of bike trips by gender for each hour of each day of the week (the heatmap can be filtered by gender)
5) A heatmap showing the number of bike trips for each type of user and gender for each day of the week, and can only filter by user and gender.
6) A heatmap showing the bide ride distribution on Geo Map. 
7) Number of Bike Rides by Gender. 

Once Done with all the above analysis I will Create a Story in Tableau ( the collection of all worksheets) to present the analysis outcome. 
 
         
### Results ( All Key Take away are impeded in the Charts Caption)




    
## *Summary*
### Advantages
 Using Pandas Tableau I was able to perform an Analysis on NYC Citi Bike and Scale this analysis to perform feasibility on City—Des Moines.  A tableau is a Powerful tool for conducting interactive and Dynamic analysis That Can be tailored to fit the needs per City and per Customer perspective.


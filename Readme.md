# Medical Appointment Data Analysis
I performed a descriptive analysis of medical appointment dataset in Brazil. The dataset 
consist of 110527 rows and 14 variables.

# Question(s) for Analysis
>- **1. Did more people show up for appointments if the appointment date was same as scheduled date?**
>- **2. Does the gender of a patient determines if he/her shows up or not ?**
>- **3. What is the relationship between showing up and age**




# Data Wrangling Process

### Accessing
**Under this section, i will be performing data wrangling processes. There will be no need for data gathering beccause the data was already provided. Some process includes:**
- Loading and Opening the data.
- Data Assessment to identify any problems in data quality or structure.
- Data cleaning to ensure the data is at high quality.

### Data Cleaning
**Here we will be cleaning up our data to make it useable for exploratory analysis**

1. To keep consistency, We have to convert all the column names to lower case and also rename the 'No-show' column to 'no_show' by using replace function.
2. Find the index number where age= -1 then dropped the row from the table.
3. Changed the datatype of both scheduledday & appointmentday to datetime.
4. Replace values > 1 with 1 in handicap column.
5. Drop all column that will not be needed for this analysis.
6. Create a new column and add to our dataset. this will show how many days a patient waits to the appointment day.
7. Drop rows where the Appointment day is behinde the scheduled day.
8. Re-arrange the dataset

# Exploratory Data Analysis
**In this section, the aim is to finding patterns and visualizing the relationships of the hospital patients who showed up or didn't show up for their appointments. The analysis carried out in this section will address the research question posed in the introductory section.**

# Conclusions
**The number of waiting days** had little effect on showing up to appointments. But with the higher number of days increased the chances of not showing up. 

Most patients who showed up for their appointments had their appointment date scheduled between 0 to 1 day.
- This means that the many of the people who showed up didn't have to wait for long for their appointment.
- The more the waiting days to an appointment, the higher the chances of not showing up.


**Gender has no effect on showed up or not** 
The number of females is almost twice that of males. This only made the analysis result more biased.


**The Age of the patients** Showed that there were high number of adult patients between ages 19-59.
- Those from Age stage 0-12, 19-59 and 59+ showed up more for their appointments.
- The patients between age 13-18 has a balance between those tha showed up and didnt show up.

### Limitation

**Higher number of females than male**
- The number of female patient is almost twice the number of males, this will make the analysis one to be biased.
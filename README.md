# DoctorNoShow
> Advanced Data Analysis Nanodegree Program
# Overview:
> In this project, you will conduct your own data analysis and create a file to share that documents your findings. You should start by taking a look at your dataset and brainstorming what questions you could answer using it. Then you should use pandas and NumPy to answer the questions you are most interested in, and create a report sharing the answers.
# Dataset:
> This dataset collects information from 100k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. Who to blame? *You can find the dataset [here](https://www.kaggle.com/datasets/joniarroba/noshowappointments).*

A number of characteristics about the patient are included in each row. The most important one if the patient show-up or no-show to the appointment.

* Be careful about the encoding of the 'Attendance' column: it says ‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up.*

* ‘Neighborhood’ indicates the location of the hospital.
* ‘Scholarship’ indicates whether or not the patient is enrolled in Brasilian welfare program Bolsa Família.
* 'SMS_Received' indecates whether or not the patient received a reminder message.
* ‘Subsidy’ indicates whether or not the patient is enrolled in Brasilian welfare program Bolsa Família.
* ‘Scheduled_Day’ tells us on what day the patient set up their appointment.
* 'Appointment_Day' tells us on what date was the appointment.
* 'Hipertension', 'Diabetes', 'Alcoholism', 'Handicap' columns: 1 if the pateint Infected with any of these chronic illnesses and 0 if not.

# Data Wrangling:
> After assessing the data visually and programmatically, the follwing issues were found and cleared:
*Quality Issues:*

* erroneous data type of (Gender, Scheduled_Day, Appointment_Day, Subsidy, Hipertension, Diabetes, Alcoholism, Handicap, SMS_Received, Attendance) columns.
* inaccurate data. (Age < 0), (Handicap Values > 1), (some appointment dates are before the schudled dates)
* inconsistent dates in Appointment_Day column and Scheduled_Day column.
* duplicated data.

*Tidness Issues:*

* 1 variable (Diseases) is divided into 4 columns (Hipertension, Diabetes, Alcoholism, Handicap)

# Conclusions:
> Although most of them made it to their appointment, there might be several effects on the reason why people miss their doctor's appointment.
* Timing Effect:

Hence, I noticed from the graphs the increase in scheduled appointments in June 2016 so, I searched the internet on what was going on then in Brazil and I found out it was the outbreak of the Zika virus. maybe not all the recorded were for the infected... but surely the epidemic made them more aware of the importance of their general health.
* Gender and Age:

Not surprising that the graphs show what looks like women are more committed but do not jump to conclusions, that does not mean men are less caring. It is only because women are much of the population.
So, let us consider the ages then; teens are the least committed, maybe it is just the nature of this age stage ... carless life :)
Adults, on the other hand, are the most committed because they are grown enough to know the importance of their health and punctuality. meanwhile, we cannot blame children as they do not have control over stuff like this it is the parent's fault.
* Do you remember me?

Another important factor is the waiting time, we can see that many of them are committed when the waiting time is up to a week even if they did not receive a reminder SMS. And the least committed are those with waiting time up to 6 months!
like who would remember an appointment 6 months later! maybe they don't even need that appointment anymore. however, receiving an SMS for waiting times more than 10 days may help.
* They know the pain...

It is sad to see that people with a history of chronic diseases are less committed to comparing to those who don’t... maybe they had enough injections and are just tired of lots of medications? we need to look after them more closely, especially those who are not registered in the Bolsa Família subsidy as they might not be able to afford the treatment expenses.
# Limitations:
1. the most important thing is it was not clear if this appointment was a dentist, a cardiologist, or other!
2. women are already a majority in the ample so we cant decide if committing to the appointment is related to gender or not.
3. most of the data collected were nominal so we couldn't make many inferential tests and we can't also show a strong correlation between them.
4. we don't have many details on some factors; for example, some poor are registered in Bolsa Família but that doesn't state that others are rich enough to afford the fee.

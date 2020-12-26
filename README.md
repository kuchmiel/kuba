# Dataset
Ford GoBike is a regional public bike sharing system in the San Francisco Bay Area, California. Bay Wheels is the first regional and large-scale bicycle sharing system deployed in California and on the West Coast of the United States with nearly The dataset used for this exploratory analysis consists of monthly individual trip data in CSV format covering the greater San Francisco Bay area.

# Data wrangling process:
fix multiple fields that are not in the correct dtype, i.e. start_time, end_time should be datetime type, user_type and member_gender should be categorical data type, etc
add new columns for trip duration in minute, trip start date in yyyy-mm-dd format, trip start hour of the day, day of week and month
add a new column calculating riders' age from 'member_birth_year'
cast 'member_birth_year' and 'member_age' to integer instead of float type
cast 'start_dayofweek' to category dtype

# Summary of Analysis
The number of trips has its peak around 8-9am and 5-6pm during a day, there were more trips on work days (Mon-Fri) compared to weekends. Summer time was the most popular season of a year, because of the weather. The duration of trips is shorter from Monday through Friday compared to weekends.

Most riders were male subscribers who did not use bike share for all trips. Most members were around 15 to 40 years old, as the age gets older, bike usage dropped significantly. Subscribers have much shorter trips than customers. 

There are more subscribers using bikes than customers. Subscribers use the bike sharing system for going to work and therefore most trips were on work days (Mon-Fri) and especially during rush hours (when going to work in the morning and getting off work in the afternoon), whereas customers ride for fun in the afternoon or early evenings over weekends. Subscribers usage has its peak in rush hours when people go to work in the morning and getting back home in the afternoon. Similar pattern was not observed among customers who tend to ride most in the afternoon or early evening for a different purpose than the subscribers.

# Insights for Presentation
Subscribers use the system heavily on work days i.e. Monday through Friday. On the other hand customers ride a lot on weekends, especially in the afternoon. Many trips are concentrated around 8-9am and 5-6pm on work days for subscribers, but customers tend to use more in the late afternoon around 5pm Monday to Friday. The efficient/short period of usage for subscribers corresponds to their high concentration on rush hours Monday through Friday, indicating the use is primarily for work commute. The more relaxing and flexible pattern of customer use shows that they're taking advantage of the bike sharing system quite differently from the subscribers, heavily over weekends and in the afternoon, for city tour or leisure purpose probably.

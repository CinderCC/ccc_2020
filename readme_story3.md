# Story 3 is about that How many tweets mentioned COVID-19 or financial pressure or pressure and are these clustered in certain areas.

## e.g. Area's population influcences the low income households 
##      Households in which state is experiencing greater financial pressure during the COVID-19              
              
### The MapReduce Query can return the total numbers of low income households in each state.
### The data of low income households is now sorted by states, but in database, their local government areas are also recorded.
### So if you want, you can also sort them by LGA. 
1. tweets_harvester3.py：    
  Upload aurin and tweets data to the database. Twitter API is StreamingAPI.   
  The filter keywords are "financial pressure", "pressure" and "covid-19".
2. dataProcess.py:  
  Add my MapReduce query part from download datasets from Aurin   
3. flaskPart.py:   
  Add a GainData3part to display my results sorted by states.   
  The URL is "/travis_app/gain_data/<region>".   

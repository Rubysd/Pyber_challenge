# Pyber_challenge

# Overview of the analysis

Based on the Python skills I have been acquiring over the last few weeks and my knowledge of Pandas, this analysis created a summarized DataFrame of ride-sharing data by city type. Then, with Pandas and Matplotlib, a multi-line chart was created showing the total weekly rates for each type of city. Lastly, I made a written report that summarizes how the data differs by city type and how PyBer decision makers can use those differences.

# Results

# RIDES FOR EACH CITY TYPE
![image](https://user-images.githubusercontent.com/86340630/126987639-7d91f907-a288-4ffb-9af5-5fa61cdef4d3.png)

# TOTAL DRIVERS FOR EACH CITY TYPE
![image](https://user-images.githubusercontent.com/86340630/126987760-2f92e4d6-8bdf-4fb0-9c2d-ac7ab9e75b66.png)

# TOTAL AMOUNT OF FARES FOR EACH CITY TYPE
![image](https://user-images.githubusercontent.com/86340630/126987823-f64dfbca-16dc-44ea-80db-8565e3976c92.png)

# THE AVERAGE FARE PER RIDE FOR EACH CITY TYPE
![image](https://user-images.githubusercontent.com/86340630/126988561-b04aedcc-2af6-4989-8b54-036b1133c6af.png)

# THE AVERAGE FARE PER DRIVER FOR EACH CITY TYPE
![image](https://user-images.githubusercontent.com/86340630/126988640-c14a0428-b960-4677-8982-0b1ef88a6e6e.png)

# CREATE A PYBER SUMMARY DATAFRAME
![image](https://user-images.githubusercontent.com/86340630/126988713-ecd7db35-7e0f-4665-ba1a-8ab658d74343.png)

# CLEANING UP THE DATAFRAME. DELETE THE INDEX NAME
![image](https://user-images.githubusercontent.com/86340630/126988782-403ed450-5b1e-4859-b64d-9ba7ab278a14.png)

# FORMAT THE COLUMNS
![image](https://user-images.githubusercontent.com/86340630/126988935-a1539fde-d144-4453USING GROUPBY() T

# READ THE MERGED DATAFRAME
![image](https://user-images.githubusercontent.com/86340630/126989034-75ae163d-b4ed-4d09-99cb-f7ba319dc882.png)

# USING GROUPBY() TO CREATE A NEW DATAFRAME SHOWING THE SUM OF THE FARES 
# FOR EACH DATE WHERE THE INDICES ARE THE CITY TYPE AND DATE.
![image](https://user-images.githubusercontent.com/86340630/126989209-21bd9e47-4123-4a67-8a31-2b57ade44684.png)

# RESET THE INDEX ON THE DATAFRAME YOU CREATED IN 1. THIS IS NEEDED TO USE THE 'PIVOT()' FUNCTION.
# DF = DF.RESET_INDEX()
![image](https://user-images.githubusercontent.com/86340630/126989358-e58cc05f-1e21-4742-9ff0-33deccb9cd29.png)

# CREATE A PIVOT TABLE WITH THE 'DATE' AS THE INDEX, THE COLUMNS ='TYPE', AND VALUES='FARE' 
# TO GET THE TOTAL FARES FOR EACH TYPE OF CITY BY THE DATE
![image](https://user-images.githubusercontent.com/86340630/126989527-fcf4fa5a-11bb-48c8-b987-ec10b0192a45.png)

# 6. SET THE "DATE" INDEX TO DATETIME DATATYPE. THIS IS NECESSARY TO USE THE RESAMPLE() METHOD IN STEP 8. # DF.INDEX = PD.TO_DATETIME(DF.INDEX)
# 7. CHECK THAT THE DATATYPE FOR THE INDEX IS DATETIME USING DF.INFO()
![image](https://user-images.githubusercontent.com/86340630/126989627-e95ba900-c225-4caa-a8d2-210f01c91104.png)

# 8. CREATE A NEW DATAFRAME USING THE "RESAMPLE()" FUNCTION BY WEEK 'W' AND GET THE SUM OF THE FARES FOR EACH WEEK.
![image](https://user-images.githubusercontent.com/86340630/126989733-a4842d0c-7acf-44e3-a362-8ef49f5a42a3.png)

# 8. USING THE OBJECT-ORIENTED INTERFACE METHOD, PLOT THE RESAMPLE DATAFRAME USING THE DF.PLOT() FUNCTION.
![image](https://user-images.githubusercontent.com/86340630/126989787-86244a01-176d-4479-80f6-788851db193a.png)

# THERE IS A STATEMENT SUMMARIZING THREE BUSINESS RECOMMENDATIONS TO THE CEO FOR ADDRESSING ANY DISPARITIES AMONG THE CITY TYPES
It might be useful to delve into additional analysis to include geographic size, population and social conditions, travel distances.

Access to the PyBer service could be improved in areas that need it most, and this in turn will involve finding the right balance between incentives for more passengers to join and charging for the correct fare that will motivate passengers to choose the application. PyBer as the first choice for your travels.

We can observe based on the data in the tables in the most underserved neighborhoods, PyBer's ridesharing services do not select the first option to travel, since the rates are quite high.


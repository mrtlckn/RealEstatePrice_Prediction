# RealEstatePrice_Prediction
->The purpose of this project is:
    to make an accurate estimate of the houses based on the data in the house_prices.csv file.

 Quick look our data
<br>![image](https://user-images.githubusercontent.com/83788186/174433751-4d8635ee-8b68-46bc-b272-6d8b57f2a130.png) </br>

# **1- Data Cleaning**
We have some issue about our data,like ;

"First Problem ('size') have 2 different value but that value actually same thing"
<br> ![image](https://user-images.githubusercontent.com/83788186/174433809-68394175-13cf-4adb-9637-8090003c36de.png) </br>


"Second Problem (total_sqft)"
<br>![image](https://user-images.githubusercontent.com/83788186/174433829-ca5961e1-22b7-428a-9834-0bbfbef0dd17.png) </br>

Let's fix this issue.


# **2-Feature Engineering**
We need to apply dimensionality reduction technique here to reduce number of locations.
if location_stats <= 10 then drop from location
<br>![image](https://user-images.githubusercontent.com/83788186/174433951-e3b80caa-b33a-4ad3-9c8c-d2d600bbaf41.png)</br>

# **3-Outlier Removal**
<br>![image](https://user-images.githubusercontent.com/83788186/174433988-828747c7-2505-4aa8-b120-cbe0302bf3bc.png)</br>

<br> ![image](https://user-images.githubusercontent.com/83788186/174434045-f8631cf5-802c-42ae-b8f9-aa7e9bf76cfd.png) </br>

# **4- Model Building**

With;
<br>**Linear Regression score** : 0.8452277697874362 </br>
<br>**K-Fold score with Linear Regression** :np_split_5([0.82430186, 0.77166234, 0.85089567, 0.80837764, 0.83653286])</br>

**GridSearchCV** : 
<br> ![image](https://user-images.githubusercontent.com/83788186/174434210-b2b378d8-0efc-49e9-8eb5-06c08074f9f8.png) </br>



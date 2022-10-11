# Bike Sharing Demand Prediction
<!--  Outline a brief description of your project. -->
In this project, we understand the variables that affect the demand of bikes on a bike sharing platform. We also create a Linear Regression model to predict the demand for bikes.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
<!--
- Provide general information about your project here.
- What is the background of your project?
- What is the business probem that your project is trying to solve?
- What is the dataset that is being used?
-->
We are trying to determine the most significant variables that affect the demand for shared bikes. The data has been provided by US bike sharing provider BoomBikes. BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. 

This project aims to determine the factors which can help the company take corrective measures to increase the demand and boost revenue. We are trying to model the demand for shared bikes with the available independent variables. It will be used by the Boombike management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

The dataset contains the following variables and the details of those is given in the Readme.txt file as well

	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered
  
  We to use `cnt`as the target variable.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Here is the list of variables that are most significant based on the value of its coefficient

![image](https://user-images.githubusercontent.com/111374919/195031094-171d21a3-7d9c-4c6f-ada3-8b743f20d298.png)

Based on this we can say that the weather parameters such as temperature, humidity, season and weathersit are the most important factors. Together it is something that the company can look at to predict the demand for bikes. Also the variable `yr` also has high coefficient and it implies that the demand for the bikes in the next year will be higher than last year even if all the other parameters are kept constant. This could be attributed to growing population in the cities year on year.
- Model metrics
  - r2 score
    - Training data 0.84
    - Test data 0.78
  - adjusted r2 score (Training data) -0.837
- Model Prediction

![image](https://user-images.githubusercontent.com/111374919/195033112-6f8d16bc-2d96-49e2-b4de-d764b4254576.png)
![image](https://user-images.githubusercontent.com/111374919/195034183-0ce2d10b-60fe-4776-ae72-469e5b90a3c2.png)
![image](https://user-images.githubusercontent.com/111374919/195034246-6d24f0fc-f88e-47e3-8cd5-5404879a570b.png)
![image](https://user-images.githubusercontent.com/111374919/195035064-8b8382a9-3b4b-4a4d-a30d-1b2d50610fdc.png)
![image](https://user-images.githubusercontent.com/111374919/195035105-2c30e4c3-68b2-48ae-b119-47abe5aa1ad1.png)





<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
Below is the list of major packages used in this project. The complete list of packages are listed in the requirements.txt file
<!--
- library - version 1.0
- library - version 2.0
- library - version 3.0
-->
- jupyter==1.0.0
- jupyter-client==7.3.4
- jupyter-console==6.4.4
- jupyter-core==4.11.1
- jupyterlab-pygments==0.2.2
- jupyterlab-widgets==3.0.2
- matplotlib==3.5.3
- numpy==1.23.2
- pandas==1.4.3
- scikit-learn==1.1.2
- seaborn==0.11.2
- statsmodels==0.13.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- References...
  - https://pandas.pydata.org/docs/
  - https://numpy.org/doc/1.23/
  - https://stackoverflow.com/
  
  Special thanks to people who have contributed to stackoverflow questions whose answers have been really helpful for my project.
- This project was based on the Machine learning course content provided by Upgrad[Upgrad](https://www.upgrad.com).


## Contact
Created by [@shyamsundarshukla1991] - feel free to contact me!

email-shyamsundarshukla1991@gmail.com


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->

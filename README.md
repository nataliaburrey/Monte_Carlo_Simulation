[
![comprehensive-financial-planning](https://user-images.githubusercontent.com/80833988/116162743-41e3d200-a6ab-11eb-9329-7bf582c11053.jpeg)
](url)


# Challenge_5

> "For this assignment, I will create 2 financial analysis tools: financial planner for emergencies with ability to visualize their current savings and financial planner for retirement based on MonteCarlo simulation.
"

!!! Important - go to HOW TO USE to make sure you can run Jupyter Lab file correctly



- [Introduction](#Introduction)
- [Why?](#why)
- [How to Install](#how-to-install)
- [How to use](#how-to-use)
- Technologies used
    - [Libraries](#Libraries)
    - [Interfaces](#Interfaces)



## Introduction

In this Challenge I created a Jupyter notebook with financial analysis tools. First, I show the ability to make an API call to retrive data for crypto portfolio and later using Alpaca software to create personal API key for stock/bond postfolio. Based on the data I recieved and analised, I calculated the value in US Dollars for crypto part portfolio and later for stocks/bonds. Using pie plot I visualized the summary of the clients portfolio and was able to determine if current Emergency fund is sufficient.

Second part of the Challenge 5 is a financial planner for retirement. This tool forecasts the performance of client retirement portfolio in 30 years, later compares it to 10 years with another stock/bond ratio. To do this, we made an Alpaca API call via the Alpaca SDK to get historical price data for use in Monte Carlo simulations.

You can find comments for the line of code and my analysis, including the answers to the question in the Challenge instructions. 
For each line of code there is comments, necessary plot visualizations are included. 


## Why?

 This platform aims to offer clients a way to determine sufficiency of their Emergency fund, as well as a solution for their retirement portfolio based on running Monte Carlo instance twice-for 10 and 30 years. With Monte Carlo analysts we can examine the possible outcomes of real-world scenarios in an environment that’s safe and efficient and offer our client different solutions to choose from.
 



## How to install

* Save remote repo from GitHub to your computer (Desktop): in Terninal type:

```
cd desktop

git clone https://github.com/nataliaburrey/Challenge_5.git
```
now you can find repo on your desktop


* Open a Jupyter Lab: In Terminal type command

```
jupyter lab
```

* In Jupyter Lab access saved repo folder 
* Choose [ financial_planning_tools.ipynb ] file to see the analysis report.



## How to use

In order to succesfully run the file you have to generate your own Alpaca key and save it to .env file. Those files are hidden so Hold down the Command, Shift and Period keys (for Mac) to be sure you have it in the same folder as Jupyter Lab notebook

```
 cmd + shift + [.]
```
To generate Alpaca key you have to create your own account and request a new key. Save it in .env file, make sure to name the variables ALPACA_API_KEY and ALPACA_SECRET_KEY 
```

ALPACA_API_KEY = '<your key>'
ALPACA_SECRET_KEY = '<your key>'

```

[
<img width="1073" alt="Screen Shot 2021-04-26 at 3 35 05 PM" src="https://user-images.githubusercontent.com/80833988/116161176-2aefb080-a6a8-11eb-9b6d-c16dbf723814.png">
](url)

Those steps are nessesary to maintain a security of private information. 


## Technologies used

### Libraries


We are using Pandas- a software library written for the Python programming language for data manipulation and analysis.
The following libriries has to be imported:

```
import os
import requests
import json
import pandas as pd
from dotenv import load_dotenv
import alpaca_trade_api as tradeapi
from MCForecastTools import MCSimulation

%matplotlib inline
```

In particular, Pandas offers data structures and operations for manipulating numerical tables and time series. It is free software released under the three-clause BSD license.

> " Written in: Python, Cython, C .  
Original author(s): Wes McKinney. . 
License: New BSD License
"




### Interfaces

* Jupyter Lab
* GitHub
* You can download Anaconda packadge on MacOC [HERE](https://www.anaconda.com/products/individual)
Make sure to use following packedge:

[
![anaconda_python37](https://user-images.githubusercontent.com/80833988/113497395-828b6980-94b8-11eb-918c-df4a446f817d.png)
](url)

* Alpaca (https://alpaca.markets/)




## Helps recruiters

* The project was created in collaboration with Berkeley Fintech Bootcamp team: Allan Hall, Joel Gonzales, Siege.
* Tutor Lavina Tang helped me to polish my code and tought me how to run separate parts of code to see if it works every step.
* AskBCS Learning Assistant was used to troubleshoot some of the accuring problems outside of the classroom

---

Feel free to contact me via channels

* Email:(nataliaburrey@gmail.com) 
* LinkedIn: (https://www.linkedin.com/in/natalia-burrey-181822175/)



---

* License

MIT

# mars_challenge


#Description

In this project I used my knowledge of web-scraping to create two files about Mars, one is about Mars weather and the other is about news articles related to Mars. 

To get the information about Mars news articles I used Splinter and BeautifulSoup. First, I extracted all of the text elements from the webpage and then I created a for loop to extract the articles titles and preview text from the webpage all into one list.  

To get the information about Mars weather, I again used Splinter and BeautifulSoup to extract information from the webpage. The data was scraped from a table on the website and then stored in a Pandas DataFrame. However, when the DataFrame was created all the values were stored as objects, so I had to change the datatypes for most of the columns in order to move forward with the analysis of the data. The specific questions that I worked to answer through my data analysis are listed in the code, section 5. Additionally, the answers to the analysis questions are found in this same section. Finally, the last portion of my code exports the DataFrame and saves it to a csv file titled, “mars_weather_dataframe.csv”. 

#Visuals

Plot of average temperature by month
![image](https://github.com/kbrantner/mars_challenge/assets/117327499/27989bfe-5e3d-41db-a262-d0a161da99e5)

 
Plot of the hottest and coldest months on Mars
![image](https://github.com/kbrantner/mars_challenge/assets/117327499/95c77e32-854d-496a-928f-f627934f7ff1)

 
Plot of the average pressure on Mars by month
![image](https://github.com/kbrantner/mars_challenge/assets/117327499/3be4fed4-ec98-4eab-abae-b8f9138a2c0a)

 
Plot that helps determine the number of Earth Days in a Martian year
![image](https://github.com/kbrantner/mars_challenge/assets/117327499/4977ed0d-c9b6-4f3a-ac8f-7e4eabf15087)





#Installation

To work with Splinter and BeautifulSoup for web-scraping and to create the graphs:
from splinter import Browser
from bs4 import BeautifulSoup as soup
import matplotlib.pyplot as plt
import pandas as pd


#Support

If help is needed with web-scraping, I recommend searching Stack Overflow for the answers to specific questions.  

#Authors and acknowledgment

This project was completed by Kelsey Brantner. I received help with the “part_2_mars_weather_kb” file with how to parse the data in step 3 using split("\n"). I also referenced the following link to understand how to covert the first row to the column titles https://stackoverflow.com/questions/26147180/convert-row-to-column-header-for-pandas-dataframe.  

#Resources

According to the files’ source site, “The Mars News website is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from NASA's Mars website in November 2022. Images are used according to the https://www.jpl.nasa.gov/jpl-image-use-policyJPL Image Use Policy, courtesy NASA/JPL-Caltech”

#Project status

At this time, the project is considered complete. 

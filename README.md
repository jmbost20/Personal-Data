# Personal-Data

#### ***For Privacy Reasons, the full .py, .ipynb, and commensurate data will not be uploaded, but instead screenshots will be provided.

#### Project Goal 
Use free available tools to create a sandbox system for tracking various behaviors.

### Overview
This project uses many products from Google Suite including Google Forms and Google Sheets to enable control in crafting of the project. 
The APIs of these products are utilized to streamline the retrieval of personal data to then be analyzed by the preferable data analytics softwares.

##### Table of Contents  
1. [Data Collection](#Data-Collection)  
2. [Data Processing](#Data-Processing)  
3. [Returnables](#Returnables)  
4. [Conclusions](#Conclusions)

<a name="Data-Collection"/>
<a name="Data-Processing"/>
<a name="Returnables"/>
<a name="Conclusions"/>



## Data Collection

With collecting personal/ behavioral data, there are a variety of free apps and websites; however, while most of these tools will allow one to export the csv of the user's data, the products can have restrictions on what exactly can be tracked in the first place. Using Google Forms provides what variables to control, and ensures the entire pipeline is free (granted that one has access to a phone and internet).

### Google Drive Interface
![Example](https://github.com/jmbost20/Personal-Data/blob/main/github.png)

The first level of interacting with this system is to create a main directory to interact with all of the different google forms
* Everything is stored within the same folder to ensure ease of use (A folder can be pinned and easily opened on the google drive app)
* Grouping variables into forms is kind of an art, but it is best to keep in mind end result goals like making it convenient to view on mobile devices.

### Google Forms Interface

![Example](https://github.com/jmbost20/Personal-Data/blob/main/Structural-Question.png)


It is to group similar variables into the same form. If all the variables that are being tracked were put in different forms, it could take longer to scroll and find the applicable form, and by having similar behaviors grouped, the variables are processed easier.



For this form, each variable is grouped


## Data Processing

#### ***There are tons of different ways to manage initial data. There not one best way!
#### ***Data must first be extracted from Google using either the Google Forms API or the Google Sheets API. This project made use of the forms API.


### Packages

Photo HERE!!!
Some of these packages are more niche and take some work to install

### API Calls

![Example](https://github.com/jmbost20/Personal-Data/blob/main/APIs.png)

This is the code that was used to access the APIs


## Returnables

### Options
After the initial data is extracted from google, there are a variety of free softwares available to use for individual purposes. As there is no one best process for representing one's data, a list will be provided of pro's and cons
* Google Sheets
  * Pros
    *   
  * Cons
* Excel
* Tableau- great for dashboards

# Conclusions

This tool is meant to be provide maximum flexibility for data tracking while reducing inconvenience that more manual methods for data tracking would incur (like tallying with pen/ paper). All in all, this system is a starting point or a backbone to then build bigger, better systems on top of: whether that means dediced iOS apps, web apps, or GUIs for collecting data, or that means focusing on the latter end of the Data Science process and integrating other data analytical softwares.


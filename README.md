# Personal-Data


#### Project Goal 
Use free available tools to create a sandbox system to enable the user to dynamically update and choose what variables they track.

### Overview
This project uses many products from Google Suite including Google Forms and Google Sheets to enable control in crafting of the project. 
The APIs of these products are utilized to streamline the retrieval of personal data to then be analyzed by the preferable data analytics softwares.

##### Table of Contents  
1. [Data Collection](#Data-Collection)  
2. [Data Processing](#Data-Processing)  
3. [Deliverables](#deliverables)  
4. [Conclusions](#Conclusions)

<a name="Data-Collection"/>
<a name="Data-Processing"/>
<a name="Deliverables"/>
<a name="Conclusions"/>



## Data Collection

With collecting personal/ behavioral data, there are a variety of free apps and websites; however, while most of these tools will allow one to export the csv of the user's data, the products can have restrictions on what exactly can be tracked in the first place. Using Google Forms provides what variables to control, and ensures the entire pipeline is free (granted that one has access to a phone and internet).

### Google Drive Interface
![Example](https://github.com/jmbost20/Personal-Data/blob/main/github.png)

The first level of interacting with this system is to create a main directory to interact with all of the different google forms
* Everything is stored within the same folder to ensure ease of use (A folder can be pinned and easily opened on the google drive app)
* Grouping variables into forms is kind of an art, but it is best to keep in mind end result goals like making it convenient to view on mobile devices.

### Google Forms Interface


#### Structural Questions

![Example](https://github.com/jmbost20/Personal-Data/blob/main/Structural%20Question.png)

 
<br />

Many of the forms have structural questions that serve to direct what other questions to ask. The above is the most general structural question, used in every form to validate the type of entry. The type of entry can be implied by other information, like how the questions are answered, but for time bound questions, this question informs properties of the variable.
<br />
<br />
For example, if the question is answered "Automatic", then in processing the form takes the timestamp of the form and uses that to calculate the total time of the behavior. If the question is answered "Manual" (either type), then the Timestamp is not used and instead, the manual time entry is converted to a date-time and used as the end point. 



#### General Data Collection
![Example](https://github.com/jmbost20/Personal-Data/blob/main/Form%20Questions.png)

These questions are just examples of types of variables that one can track. The power of this system is that one can be very dynamic in what is deemed worthy of inclusion. In creating these question, the end result should be entertained, "How is this going to be encoded to create insights".

#### Regex Implementation



![Example](https://github.com/jmbost20/Personal-Data/blob/main/Screen%20Shot%202022-10-14%20at%208.04.17%20PM.png)

The lower portion illustrates where the regex was used.

![Example](https://github.com/jmbost20/Personal-Data/blob/main/Screen%20Shot%202022-10-14%20at%208.04.48%20PM.png)

The Above is the exact characters and digits that were used. 

###### Best Practice:
It is best to group similar variables into the same form. If all the variables that are being tracked were put in different forms, it could take longer to scroll and find the applicable form, and by having similar behaviors grouped, the variables are processed easier.


## Data Processing

#### ***There are tons of different ways to manage initial data. There not one best way!
#### ***Data must first be extracted from Google using either the Google Forms API or the Google Sheets API. This project made use of the forms API.


### Packages

![Example](https://github.com/jmbost20/Personal-Data/blob/main/Packages.png)

* Could use other API Packages, but used these bc they provided clear level of abstraction
* Some of these packages are more niche and take some work to install.
* Be cautious with uploading keys

### API Calls

![Example](https://github.com/jmbost20/Personal-Data/blob/main/APIs.png)

This is the code that was used to access the APIs, and return the data. Again, there are two main APIs to use here, the Gsheets and GForms. Either way, it is just important process it appropriately.

<br />


## Deliverables

### Options
After the initial data is extracted from google, there are a variety of free softwares available to use for individual purposes. As there is no one best process for representing one's data, a list will be provided of pro's and cons. Again, the software chosen depends on purpose, this is just a very general comparison.
* Google Sheets
  * Pros
    *   *Free, Great Mobile Access*
  * Cons
    *   *Lacks some more advanced features*
* Excel
  * Pros
    *   *Buff with features*
  * Cons
    *   *Costs Money to use*
* Tableau/ PowerBI
  * Pros
    *   *Incredible Dashboards*
  * Cons
    *   *Costly, Learning Curves*

# Conclusions

This tool is meant to be provide maximum flexibility for data tracking while reducing inconvenience that more manual methods for data tracking would incur (like tallying with pen/ paper). 
<br />
<br />
All in all, this system is a starting point or a backbone to then build bigger, better systems on top of: whether that means dediced iOS apps, web apps, or GUIs for collecting data, or that means focusing on the latter end of the Data Science process and integrating other data analytical softwares.


# Tourism-Market-Segmentation
---
This Repository contains Market Segmentation project done as part of Data Science Internship at Feynn Labs.
#### Project Status: [Completed]

### Objective
The purpose of this project is to analyse the Tourism market and come up with a feasible strategy to enter the market targeting the segments most likely to use their services.

### Methods Used
* Statistics 
* Machine learning(Unsupervised Learning)
* Data Visualization 
* Data Preprocessing
* Segmentation of Variables
* Profiling the Segments
* Choosing the Target Segments

### Technologies
- Tools: PowerBI, Jupyter
- Language: Python
- Libraries: Pandas, Numpy, Matplotlib, Sklearn, Seaborn, Scipy.


### Project Description
#### Data Collection
- Initially Data has Been collected from kaggle which consist of features [Circle, Name of Monument, Domestic(2017-17), Foreign(2016-17), Domestic(2017-18), Foreign(2017-18), Domestic Percentage growth(2016-17/2017-18, Foreign Percentage growth(2016-17/2017-18].
- Include manually collection of data with respect to Circle and Name of Monument.[Airport(in km),Railway (in km)].


#### Defining Knock Criteria and Segmentation Criteria
* Knock Out Criteria: Segment must be 
   - Relevant
   - Measurbale 
   - Accessible
   - Large Enough
   - Homogenous
 
* Segmenataion Criteria
   - Behavioral Segmentation
      - More no. of tourist
      - Attractivenss Sightseeing
      - Closesness to nature
      - Adventure
   - Psychographic Segmentation:
      - Less Distance
      - Connectivity
      

#### Data Visualization and Preprocessing
- All feature are positively skewed implies presence of outliers. Confirmed outliers by plotting the box and whisker plot.
- Removed one of the Vadodara circle feature because it didn't contained the tourist value.
- Removed Leh Circle because the Railway feature could not be imputed as there no railway station is less than 400km of range.
- Imouted all missing values with zeron in Airport and Railway Feature because the Momumnets we too close to the Ariport, Railway.(less than 1 km).
- Used Different transformation method to remove the skewness and treat the outliers. PowerTransformer Performed very well and reduces the skewness as well treats the outliers. Standardie feature having mean 0 and variance 1.
- Plotted the correlation plot to consider only less correlated values

#### Approaches
Different Approaches used:
- Naive Bayes
- Hierarchial Agglomerative Clustering
- K-Means Clustering.

Out of these K-Means was chosed and used for further analysis.

#### Clustering
- Domestic 2016-17 and Foreign 2016-17 features were used to cluster.
- No. of cluster chosed for analysis is 4 based on Elbow plot and  Silhouette analysis.
- Silhouette Score for 4 cluster is = 0.39
![output](https://user-images.githubusercontent.com/69076815/134291943-dc89b499-9058-4113-a110-8cc4479553e8.png)

![output](https://user-images.githubusercontent.com/69076815/134292020-ea96cc88-d1b6-4b0c-b2b9-096ab668b7ef.png)

- Based on plots and Knock out Criteria Cluster 2 and Cluster 1 was chosen for further anlysis.(Take a look into notebooks> model-training K-Means).
- Based on Knock out Criteria i.e., Segment must be Large and Homogenous, Cluster 2 was choosen as the perfect cluster.
- From Cluster 2 Circle - Agra, Bhopal, Dharwad were chosen to be place for opening the hostel chain.

### Getting Started
- Clone this repo.
- Download the unprocessed data(folder - data>Tourism.csv)
- Download the two notebooks(notebooks> eda.ipnb, model-training K-Means.ipynb)
- First run the eda notebook and then the model-training K-Means.ipynb to get results in Jpyter Notebook


### Members of the Project
- Malhar Lumbhani
- Aryan Sharma
- Ankur Bhayana
- Ritik kumar Jain






<!-- # Project Name
This project is a part of the [Data Science Working Group](http://datascience.codeforsanfrancisco.org) at [Code for San Francisco](http://www.codeforsanfrancisco.org).  Other DSWG projects can be found at the [main GitHub repo](https://github.com/sfbrigade/data-science-wg).

#### -- Project Status: [Active, On-Hold, Completed]

## Project Intro/Objective
The purpose of this project is ________. (Describe the main goals of the project and potential civic impact. Limit to a short paragraph, 3-6 Sentences)

### Partner
* [Name of Partner organization/Government department etc..]
* Website for partner
* Partner contact: [Name of Contact], [slack handle of contact if any]
* If you do not have a partner leave this section out

### Methods Used
* Inferential Statistics
* Machine Learning
* Data Visualization
* Predictive Modeling
* etc.

### Technologies
* R 
* Python
* D3
* PostGres, MySql
* Pandas, jupyter
* HTML
* JavaScript
* etc. 

## Project Description
(Provide more detailed overview of the project.  Talk a bit about your data sources and what questions and hypothesis you are exploring. What specific data analysis/visualization and modelling work are you using to solve the problem? What blockers and challenges are you facing?  Feel free to number or bullet point things here)

## Needs of this project

- frontend developers
- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- writeup/reporting
- etc. (be as specific as possible)

## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](Repo folder containing raw data) within this repo.

    *If using offline data mention that and how they may obtain the data from the froup)*
    
3. Data processing/transformation scripts are being kept [here](Repo folder containing data processing scripts/notebooks)
4. etc...

*If your project is well underway and setup is fairly complicated (ie. requires installation of many packages) create another "setup.md" file and link to it here*  

5. Follow setup [instructions](Link to file)

## Featured Notebooks/Analysis/Deliverables
* [Notebook/Markdown/Slide Deck Title](link)
* [Notebook/Markdown/Slide DeckTitle](link)
* [Blog Post](link)


## Contributing DSWG Members

**Team Leads (Contacts) : [Full Name](https://github.com/[github handle])(@slackHandle)**

#### Other Members:

|Name     |  Slack Handle   | 
|---------|-----------------|
|[Full Name](https://github.com/[github handle])| @johnDoe        |
|[Full Name](https://github.com/[github handle]) |     @janeDoe    |

## Contact
* If you haven't joined the SF Brigade Slack, [you can do that here](http://c4sf.me/slack).  
* Our slack channel is `#datasci-projectname`
* Feel free to contact team leads with any questions or if you are interested in contributing! -->

# Capstone: Check In 2

### Contents:
- [Project: Quote Recommender](#Project)
- [Goal: Problem Statement](#Goal)
- [Success Criteria](#SuccessCriteria)
- [Proposed Methods and Models](#MethodsModels)
- [Risks & Assumptions](#RisksAssumptions)
- [Data Source](#DataSource)
- [Preliminary EDA](#PreliminaryEDA)

<a id=Project></a>
## Project: Quote Recommender
My Capstone project will be a personal growth quote recommender. 

<a id=Goal></a>
#### Problem Statement: 
Develop a recommender that will output recommended quotes based on keywords as prompts to identify category or general gist of quote to be recommended.

<a id=SuccessCriteria></a>
#### Success Criteria
Mean Average Precision at K <br>
Mean Average Recall at K 

<a id=MethodsModels></a>
#### Proposed Methods and Models
Knowledge for how to build a recommender will be obtained from the following online courses:
 - Udemy Course 1: Building Recommender Systems with Machine Learning and AI <br> https://www.udemy.com/course/building-recommender-systems-with-machine-learning-and-ai/learn/lecture/11412656?start=150#overview 
 - Udemy Course 2: Recommender Systems and Deep Learning in Python <br> https://www.udemy.com/course/recommender-systems/learn/lecture/11686566?start=0#overview

Natural Language Processing (NLP) will be employed to process the text for similarites with the input prompt.

I will be using the scikit-surprise library http://surpriselib.com/


<a id=RisksAssumptions></a>
#### Risks & Assumptions of Data
There is a risk that the quote data does not cover a broad category since the website is centered around personal growth.

I'm assuming I will be able to easily extract quotes with the h2 tag and isolate the h2 text that is surrounded in quotations to separate out the quotes from other text.

<a id=DataSource></a>
#### Data Source
Data will be obtained through web scraping the website https://www.brainpickings.org/ which has over 13 years worth of weekly posted qoutes. The original site I intended to use forbids scraping, despite having seen data from others who have scraped the site.  Alternately, there are several quotation books on the website gutenberg.org, for example: https://www.gutenberg.org/files/21130/21130-h/21130-h.htm.

<a id=PreliminaryEDA></a>
### Preliminary EDA
In progress











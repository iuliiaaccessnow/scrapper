
# Current progress:
- first in terminal
```
pip install -r requirements.txt
```
- RestoTAPerso spider can be used to scrapped data for the neighborhoods change url in def start_requests(self) from line 20 to scrape different url
```
scrapy crawl RestoTAPerso --overwrite-output=TA_reviews/scrapped_data/scrapped_data.jl
```
- Toronto spider let you scrape restaurant names and addresses for the neighborhood, change the url in def start_requests(self) from line 15 to scrape different url. There is a bug - scrapes only one page
```
scrapy crawl Toronto --overwrite-output=TA_reviews/scrapped_data/scrapped_data.jl
```

## Below README is from https://github.com/henrique-britoleao/trip_advisor_scrap 

## Table of contents
- [Deliverable 1:](#deliverable-1-)
  * [General info](#general-info)
  * [Technologies](#technologies)
  * [Setup](#setup)
- [Deliverable 2:](#deliverable-2-)
  * [General info](#general-info-1)
  * [Technologies](#technologies-1)
  * [Setup](#setup-1)
- [Deliverable 3:](#deliverable-3-)
  * [General info](#general-info-2)
  * [Technologies](#technologies-2)
  * [Setup](#setup-2)


## Deliverable 1:

### General info
Implements a spider to crawl trip advisor looking for restaurant reviews.
	
### Technologies
Project is created with:
* Python version: 3..
* Scrapy

	
### Setup
To run this project, install it locally:

```terminal
pip install -r requirements.txt
scrapy crawl [spider-Name] --overwrite-output=TA_reviews/scrapped_data/scrapped_data.jl
```
Data from webscraping will be in ../trip_advisor_scrap/TA_reviews/TA_reviews/scrapped_data.

## Deliverable 2: 

### General info
Preprocessed data obtained in first part of the project. Main delivery in Deliverable.ipynb
Performed:
* Data cleaning
* Data exploration
* Tokenization, stemming, and lemmatization 
* TF-IDF 

### Technologies 
* Python version: 3..
* nltk
* pycld2
* Wordcloud

### Setup
Make sure to install dependencies before running the notebook. Also make sure that the steps taken in Deliverable 1 have all been taken. 
```terminal
pip install -r requirements.txt
```

## Deliverable 3:

### General info
Performed data augmentation and embedding methods on the preprocessed data from Deliverable 2. Main delivery in Deliverable3.ipynb
Performed:
* Data augmentation
* Word2Vec
* LSI
* FasText
* SVD

### Technologies 
* Python version: 3..
* gensim
* sklearn
* nltk

### Setup
Make sure to install dependencies before running the notebook. Also make sure that the steps taken in Deliverable 2 have all been taken. 
```terminal
pip install -r requirements.txt
```

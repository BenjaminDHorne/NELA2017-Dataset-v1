# NELA2017 Dataset

**This dataset is now hosted on Harvard Dataverse, along with other news datasets: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/ZCXSKG**

NELA2017 Data Set Version 1

If this data set is used in publication, please cite the following paper:

Horne, Benjamin D., et al. "Sampling the News Producers: A Large News and Feature Data Set for the Study of the Complex Media Landscape." ICWSM 2018

--------------------------------------------------------------------------------
Due to the size of the data, the folders are compressed and split. These can be zipped back together using WINRAR, and then extracted.

This data set contains news articles from 92 news sources between April 2017 and October 2017. 

The folder structure is as follows: month -> day -> source -> articles

Each article file is a JSON file titled in the following format: source-date-first100wordsoftitle.txt

Each JSON file is a dictonary with the following feilds:
	- content - the text from the body of the article
	- title - the text from the title of the article
	- source - the source of the article
	- author - the journalist who wrote the article, if the
	- information is available in the web page meta data
	- published - the UTC time stamp of publication according
	to the web page
	- link - the url used to scrape the article (RSS feed or web
	page depending on how the source was scraped)
	- html - the full HTML of the article page stored as unicode
	
In the folder "supplementary data", there are feature vectors (formated as a csv) for each news article with the filename as the vector id. Each vector has 130 features on the body text and title text separately. Details about these features can be found in our ICWSM 2018 paper.

New versions of this data set with more news sources and updated timeline can be requested at nelatoolkit.science.  

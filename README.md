# profChiou-Web-Scraper
News article web scraping script for professor Chiou's research project on the impact of the 2016 Facebook ban, as it pertains to the anti-vaxx movement. 

.PDF File Notes:
  - Articles appearance is adjusted from original site to accommodate .PDF format
     
     * Before .PDF export, site HTML was edited to remove any superfluous elements that would distract from the article text (e.g. text-wrapped Google Ads, sidebar navigation/ads, site masthead, etc.).

Code Notes:
  - If article listed in spreadsheet is not found online: ```#SourceNotFound ```

  - If article is found, but removed from source site: ``` #SourceRemovedFromSite ```



Library/Module Installation:
  - Newspaper - ```pip install newspaper```

Code Execution:
  - Import Libraries:
  
    - ``` from newspaper import Article```
    - ``` import re ```
  - Accessing Article Information:  
    - Declare and initialize a url variable: ``` url = INSERT_ARTICLE_LINK```
    - Declare and initialize variable "article": ``` article = Article(url)```
    - Download article to enable data extraction and manipulation: ``` article.download()```
    - Parse various article information: ``` article.parse()```
  - Extracting Article Characteristics:
    - Create a .txt file and append the text information: ``` 1. file = open("article.txt", "a") | 2. file.write(article.text)```
    - Include .txt file name in for loop (lines xx-xx) to acquire article word count
    
  

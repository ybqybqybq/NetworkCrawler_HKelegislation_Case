# NetworkCrawler_HKelegislation_Case
Using the website of Hong Kong e-Legislation as an example, Requset, Beautifulsoup, and Selenium webdriver are used to crawl the relevant pdf and rtf documents.
hkLegislation.ipynb contains two modules, data acquisition and document download. 

Url: https://www.elegislation.gov.hk/index/chapternumber?TYPE=1&TYPE=2&TYPE=3&LANGUAGE=E&p0=1
![image](https://github.com/ybqybqybq/NetworkCrawler_HKelegislation_Case/assets/71159153/43a5d9d2-9842-4217-ab2a-d0a1669eb5b1)

The function of the data acquisition module: Analyze the contents of web pages and crawl relevant resources.
   Uses the Request library to access web pages.
   Uses Selenium to wait for the loading of dynamic data.
   Uses Beautiful Soup to parse HTML pages step by step to obtain the chapter name, file name, and download links of files in different languages of each chapter. 
   Data is stored in the dataframe, the download path is manually set, and the dataframe is generated into a CSV file to facilitate data visualization and data analysis. 
The function of the document download module is: 
  Using the Request library to request the corresponding download link of the dataframe, download it to the corresponding directory, and name it according to the specified format.

The crawled results are stored in the res.csv file, with each column of the file corresponding to the value of each column of each chapter in the page.
![image](https://github.com/ybqybqybq/NetworkCrawler_HKelegislation_Case/assets/71159153/e29d3a52-2a3e-4723-ac16-25f8bc3c63ea)

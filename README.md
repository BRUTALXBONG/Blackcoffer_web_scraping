# Blackcoffer_web_scraping
## Objective
The objective of this assignment is to extract textual data articles from the given URL and perform text analysis to compute variables that are explained below. 

## Data Extraction
Input.xlsx
For each of the articles, given in the input.xlsx file, extract the article text and save the extracted article in a text file with URL_ID as its file name.
While extracting text, please make sure your program extracts only the article title and the article text. It should not extract the website header, footer, or anything other than the article text. 

NOTE: YOU MUST USE PYTHON PROGRAMMING TO EXTRACT DATA FROM THE URLs. YOU CAN USE BEATIFULSOUP, SELENIUM OR SCRAPY, OR ANY OTHER PYTHON LIBRARIES THAT YOU PREFER FOR DATA CRAWLING. 

## Data Analysis
For each of the extracted texts from the article, perform textual analysis and compute variables, given in the output structure excel file. You need to save the output in the exact order as given in the output structure file, “Output Data Structure.xlsx”
NOTE: YOU MUST USE PYTHON PROGRAMMING FOR THE DATA ANALYSIS


## Variables
The definition of each of the variables given in the “Text Analysis.docx” file.
Look for these variables in the analysis document (Text Analysis.docx):

POSITIVE SCORE
NEGATIVE SCORE
POLARITY SCORE
SUBJECTIVITY SCORE
AVG SENTENCE LENGTH
PERCENTAGE OF COMPLEX WORDS
FOG INDEX
AVG NUMBER OF WORDS PER SENTENCE
COMPLEX WORD COUNT
WORD COUNT
SYLLABLE PER WORD
PERSONAL PRONOUNS
AVG WORD LENGTH

## Output Data Structure
Output Variables: 

All input variables in “Input.xlsx”

POSITIVE SCORE,
NEGATIVE SCORE,
POLARITY SCORE,
SUBJECTIVITY SCORE,
AVG SENTENCE LENGTH,
PERCENTAGE OF COMPLEX WORDS,
FOG INDEX,
AVG NUMBER OF WORDS PER SENTENCE,
COMPLEX WORD COUNT,
WORD COUNT,
SYLLABLE PER WORD,
PERSONAL PRONOUNS,
AVG WORD LENGTH


Check out the output data structure spreadsheet for the format of your output, i.e. “Output Data Structure.xlsx”.

## How I approached the solution?
I began by examining the dataset and reviewing the tasks assigned. Subsequently, I downloaded the dataset and imported it into my Jupyter Notebook Python environment from an input Excel file. My initial step involved data extraction, where I utilized libraries such as Pandas,Numy for data manipulation and Beautiful Soup to scrape data from each URL. I then organized the extracted information into separate columns within the Excel file. Following the extraction process, I identified and extracted all relevant text elements from the URLs, storing this data in individual columns adjacent to their respective rows. 

Proceeding to data preprocessing, I focused on cleaning the extracted text, which included tasks such as removing stop words and symbols.

Subsequently, I got into the main analysis phase. This involved loading the dataset and referencing a master directory containing positive and negative words. For each extracted word, I compared it against both positive and negative word lists. Whenever a match was found, I incremented the respective positive and negative counters.

These positive and negative scores were then recorded in dedicated columns within each row of the dataset. Additionally, I implemented defined functions to compute various metrics and derived values. These functions included calculating polarity scores, subjectivity scores, and derived metrics such as the count of  words, average word length, and average words per sentence etc

Overall, this structured approach facilitated comprehensive analysis and yielded valuable insights from the dataset.




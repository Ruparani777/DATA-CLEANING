# DATA-CLEANING
Data is in 2 formats:
1.structured data.
2.Unstructred data.

Gone are the days when we used to have data mostly in row-column format, or we can say Structured data. In present times, the data being collected is more unstructured than structured. We have data in the form of text, images, audio etc and the ratio of Structured to Unstructured data has decreased over the years. 
 FOR UNSTRUCTED DATA:
1.ESCAPING HTML CHARCATERS (import from html.parser)
2.DECODING DATA(#Encode from UTF-8 to ascii
encode_tweet =tweet.encode('ascii','ignore')
print("encode_tweet = \n{}".format(encode_tweet))
#decode from ascii to UTF-8
decode_tweet=encode_tweet.decode(encoding='UTF-8')
print("decode_tweet = \n{}".format(decode_tweet)))
3.APOSTROPHE LOOKUP                                    
4.REMOVAL STOP WORDS(Stop words are the words which occur frequently in the text but add no significant meaning to it)
5.REMOVE PUNCTUATIONS
6.SPLIT ATTACHED WORDS(eg: forthe ---for the)
7.SLANG LOOKUP(eg:asap---as soon  as possible)
9.STANDARIZING WORD(eg: drivnig---driving ,misss u ---miss you)
10.REMOVAL OF URLS
ADVANCE DATA CLEANING:
1.GRAMMER CHECKING
2.SPELLING CORRECTION
NOW THE DATA IS CLEANED,U ARE READY FOR TEXT MINING:

>>>Data cleaning not only refers to removing chunks of unnecessary data, but it’s also often associated with fixing incorrect information within the train-validation-test dataset and reducing duplicates.

*The importance of data cleaning:
Data cleaning is a key step before any form of analysis can be made on it.
Datasets in pipelines are often collected in small groups and merged before being fed into a model. Merging multiple datasets means that redundancies and duplicates are formed in the data, which then need to be removed.

FOR STRUCTRED DATA :(TABULAR)
Here are some key takeaways on the best practices you can employ for data cleaning: (DONE IN  PANDAS)
>Identify and drop duplicates and redundant data
>Detect and remove inconsistencies in data by validating with known factors
>Maintain a strict data quality measure while importing new data.
>Fix typos and fill in missing regions with efficient and accurate algorithms

DATA EXPLORATION: (USING PANDAS):
1.Reading and writing data.( csv files :df=pd.read_csv()   or write ki df=to_csv() for excel use Excel in place of csv)
2.Getting preview of data frame(head or tail)
3.Rename columns of df
4.selecting columns or rows
5.Handling  missing values
6.creating new columns
7.aggregate
8.Merging/concate df
9.Applying function to elemnet,column,or df
10.basic stats

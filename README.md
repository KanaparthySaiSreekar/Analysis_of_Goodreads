About 6000 odd "best books" were fetched and parsed from Goodreads. The "bestness" of these books came from a proprietary formula used by Goodreads and published as a list on their web site.

We parsed the page for each book and saved data from all these pages in a tabular format as a CSV file. In this lab we'll clean and further parse the data. We'll then do some exploratory data analysis to answer questions about these best books and popular genres.

By the end of this lab, you should be able to:

Load and systematically address missing values, ancoded as NaN values in our data set, for example, by removing observations associated with these values.
Parse columns in the dataframe to create new dataframe columns.
Create and interpret visualizations to explore the data set
Basic EDA workflow
(From the lecture, repeated here for convenience).

The basic workflow is as follows:

Build a DataFrame from the data (ideally, put all data in this object)
Clean the DataFrame. It should have the following properties:
Each row describes a single object
Each column describes a property of that object
Columns are numeric whenever appropriate
Columns contain atomic properties that cannot be further decomposed
Explore global properties. Use histograms, scatter plots, and aggregation functions to summarize the data.
Explore group properties. Use groupby and small multiples to compare subsets of the data.
This process transforms your data into a format which is easier to work with, gives you a basic overview of the data's properties, and likely generates several questions for you to followup in subsequent analysis.

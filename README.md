Data wrangling is a broad term used, often informally, to describe the process of transforming raw data
to a clean and organized format ready for use. For us, data wrangling is only one step in preprocessing
our data, but it is an important step.
The most common data structure used to “wrangle” data is the data frame, which can be both intuitive
and incredibly versatile. Data frames are tabular, meaning that they are based on rows and columns like
you would see in a spreadsheet. Here is a data frame created from data about passengers on the Titanic
There are three important things to notice in this data frame.
First, in a data frame each row corresponds to one observation (e.g., a passenger) and each column
corresponds to one feature (gender, age, etc.). For example, by looking at the first observation we can
see that Miss Elisabeth Walton Allen stayed in first class, was 29 years old, was female, and survived
the disaster.
Second, each column contains a name (e.g., Name, PClass, Age) and each row contains an index number
(e.g., 0 for the lucky Miss Elisabeth Walton Allen). We will use these to select and manipulate
observations and features.
Third, two columns, Sex and SexCode, contain the same information in different formats. In Sex, a
woman is indicated by the string female, while in SexCode, a woman is indicated by using the integer
1. We will want all our features to be unique, and therefore we will need to remove one of these
columns.
In this chapter, we will cover a wide variety of techniques to manipulate data frames using the pandas
library with the goal of creating a clean, well-structured set of observations for further preprocessing.

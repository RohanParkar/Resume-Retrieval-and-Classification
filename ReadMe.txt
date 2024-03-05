====================================================================================================================
Resume Retrieval and Classification System
====================================================================================================================
This system is divided into two sections:
 A. Resume Retrieval using inverted index.
	This section takes a collection of resume documents in .txt format and converts it into inverted index.
	The input is in the form of query entered by the user. The resumes relevant to the input query are retrieved.
	The user can select number of the document id from displayed list to view the resume. 
	The user can segregate top5 resumes based on the query input. This is achieved using ranked retrieval.
 B. Resume Classification using Vector Space Model
	This section is capable of classifying the document provided by the user into 25 different resume profiles 
	classes.This is done using the vector space model annd cosine similarity. The program takes data from a .csv 
      file and combines all the resume data regarding a particular class together. The resume(in txt format) 
	provided by the user is checked for cosine similarity with every resume profile class. The highest ranked 
	class is determined as the resume profile for the document(resume). 

-------------------------------------------------------------------------------------------------------------------
Importing the project
-------------------------------------------------------------------------------------------------------------------
1.Download and install IntelliJ Idea Community Edition.
2.Download the'Team04_CheckPoint4.zip' file and unzip it at a desired location.
3.Select the open option at the IntelliJ Idea welcome window or select File-->Open and select the folder 
  'Resume Retrieval and Classification' from the location you unzipped the zip file.
4.Compile and run the main.java file to run the program.

-------------------------------------------------------------------------------------------------------------------
How to use the user interface?
-------------------------------------------------------------------------------------------------------------------
1.The main gui window has two options Resume Classification and Resume Retrieval.
2.Press the button to choose the option.
3.On clicking resume classification or retrieval the respective window will open.

For resume retrieval :
1. Enter the skills you want to find in a resume.
2. Hit the search button to get the list of matching resumes.
3. To view the listed resume select the number from the dropdown list below and press display.
4. To get the top 5 matching resumes hit the top 5 resumes button. You can find them in the Ranked Resume folder.
5. Refresh to search again.

For resume classification:
1.Browse and select a resume in text format.
2. Hit the classify button to get the profile of the resume.
3. View the resume profile at the bottom of the window.
4. Refresh to search again.


-------------------------------------------------------------------------------------------------------------------
Classes in Resume Retrieval and Classification
-------------------------------------------------------------------------------------------------------------------
#Main.java
It has the main class to run the program along with user interface.

#Inverted_Index_Resume.java
It has the main logic to generate the inverted index and answer the user queries.

#Vector_Space_resume.java
It has the main logic to generate the vector space model and classify the input resume.

#Rank_Search.java
It has the main logic to generate the vector space model and perform ranked retrieval.

#Merge.java
It is useful in processing the posting list of the inverted index to answer user queries.

#ParserA.java
It performs the natural language processing the data.

#FileOpen.java
It opens the resume selected by the user from the retrived resume list.

#ReadFiles.java
It is used to read the input data and stop words file.

#Stemmer
Performs porter's stemming on the input provided.

#Doc.java
Tt is a data structure to store document ids and their term weights.

#ParserB.java
It cleans the data and removes the stop words.

===================================================================================================================


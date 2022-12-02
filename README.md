# Resume-Scanner
The resume scanner ranks a candidate for a given role based on the education, experience and other information obtained on his or her resume.

## Description
It is a form of pattern matching between a job’s descriptions or requirements and the qualification of a candidate based on their resume. The main aim of ranking resumes is to decide whether to move a candidate forward – usually onto an interview or to reject them.

## Usage
```
The aim is to reduce the complexity and make it easier for companies to hire candidates by
analysing the resumes in bulk rather than manually going through them.

```

## Features

- Extracting key words
- Percentage matching for each resume
- Ranking candidates based on the features


## Deployment

**Importing all required libraries:**

- Pandas, Scikit, RegEx,

**Reading the dataset- Resume Scanner.csv(Resume Scanner.rar)**

**Handling Null values and dropping the features which are not required**

**Fetching the unique value from the 'degree' feature**

**Feature Handling of 'degree', 'links' and 'work_experience':**
- 'degree' convert into 'bachelor', 'master', and 'docterte'
- 'links' convert into 'profile'
- handling the null values of work_experience and converted it's all data into integer format

**Removing the 'degree' and 'links' from the dataset after feature handling**

**Defining the functions to calculate the rank of the resume:**
- Lemmatizer function
- Function to differentiate noun, adjective, verb, adverb,

**Opening the Job Description from the text file- Job Description.txt**

**Reading all resume's from the dataset and convert into text which will appended into a list**

**Getting the cosine score by calling cosine similarity function**

**Generating dataframe which contains the name of the candidate and the cosine score**



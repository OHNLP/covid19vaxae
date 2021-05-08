# covid19vaxae

COVID19 Vaccination Adverse Event (AE)

## Dataset
The raw data files are from VAERS (https://vaers.hhs.gov/data.html).
In this repositary, we provide the following data files:

1. `sample/`: 500 AE raw text files for annoation and developing system. 
3. `sample.csv`: The CSV format data file which contains all of the text in the `sample` folder. 
4. `large.csv`: The CSV format data file which contains much more records.

The columns in both `sample.csv` and `large.csv` are defined as follows:

| Column       | Description |
| ------------ | ----------- |
| VAERS_ID     | Unique ID       |
| AGE_YRS      | Age        |
| SEX          | Sex        |
| VAX_DATE     | Vaccination Date        |
| **SYMPTOM_TEXT** | Raw text which describes the symptom        |
| VAX_MANU     | Vaccine name        |
| **SYMPTOM**      | Identified symptom  |

The `SYMPTOM_TEXT` is the text content for each raw text file, and the `SYMPTOM` is used in the file name.
You could download all of these files here: https://github.com/OHNLP/covid19vaxae/archive/refs/heads/main.zip

## Code

There are some Jupyter notebooks for data exploration.

- data_preprocessing.ipynb: create dataset from the raw data.
- nlp_tasks: Simple NLP classification workflow.

If you don't have an local environment to run these notebook, you could use the free version of Google Colab (https://colab.research.google.com/) or Deepnote (https://deepnote.com/). The basic machine is free and good enough for running these Jupyter notebooks.

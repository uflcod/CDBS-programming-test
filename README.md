# University of Florida Community Dentistry and Behavioral Science Programming Test

The goal of this programming test is to assess some of the skills necessary for the programmer position in the [University of Florida Department of Community Dentistry and Behavioral Science](https://dental.ufl.edu/departments/communitydentistryandbehavioralscience/). 

You will have **two hours** to complete the test, and you are allowed to use any resources at your disposal. If you cannot complete an exercise, do as much as you can, and do not hesitate to email us if an exercise is not clear.   

To perform the test, you can either (1) clone this repository and fill in the answers using the `notebooks/CDBS-programming-test.ipynb` Jupyter notebook, or (2) you can download the `data/drug_info.db` SQLite database and work on the answers using your own resources.

If you decide to use the Jupyter notebook, you can return the answers to us by saving the notebook as a PDF or HTML file and emailing the files to us. You can also upload the notebook to your own Github repository and send us a link to the notebook. If you decide to upload the notebook, please use the [NBViewer](https://nbviewer.org/) website to create a URL for your notebook.

If you decide to use your own resources, you will need to email both your **code** and the **answers**  to us. Please ensure that the files are able to be opened in a standard text editor, such as Notepad, or in MS Word.



## Programming Exercises 

1. Write SQL queries to find out how many rows are in the `provider` and `prescription` tables.  

2. Write an SQL query that uses the `Prscrbr_Type` field in the `provider` table to find the unique provider types.

3. Write an SQL query to get a count for each of the unique provider types.

4. Write an SQL query that uses the `Prscrbr_Type` field in the `provider` table to create a subset of the `prescription` table that only includes prescriptions made by dental providers with the following specialties:
    - Dentist
    - Maxillofacial Surgery
    - Oral & Maxillofacial Surgery
    - Oral Surgery (Dentist only)
    
    Save the results into a dataframe. This dataframe will be used in other exercises.

5. Using the dataframe from *Excercise 4*, group the data by the `Brnd_Name` column and report how many brands are in each group.   
   Report top 5 highest brand names.
   
6. Write an SQL query to output the same information produced in Excercise 5.

7. Write an SQL query to determine how many records in the `provider` table have a null value in the `Tot_Benes` field.

8. Use a dataframe to determine how many records in the `provider` table have a null value in the `Tot_Benes` field.

9. In the `drug_name` table, the `Opioid Flag` field indicates if a drug is an opioid; Y = yes, N = no.  
  Use this information to write an SQL query that find the 10 most prescibed brand name (i.e., `Brnd_Name`) opioids in the `prescription` table, and provide a count of each brand name.

10. Use a dataframe to find the information asked for in Excercise 9.

11. Using the dataframe from *Exercise 4* that subsetted the prescriptions by speciality, find the opioids prescribed for each specialty.
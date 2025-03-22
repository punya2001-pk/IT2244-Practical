# **Pro1.bat**

- Print the current month
- Print the current date
- Print the current day

**Output**

![Pro1](https://github.com/user-attachments/assets/d8a9389a-6980-4884-8ce4-2ff58bbf96bf)

# **Pro2.txt**

- create new empty csv file
* touch abc.csv

- enter data 
* vi abc.csv

- view data
* more abc.csv

- display the first column's data
* awk -F "," '{print $1}' abc.csv

- display the first two column's data
* awk -F "," '{print $1","$2}' abc.csv

- display the file data
* cat abc.csv

- display number of columns
* awk -F , '{print NF; exit}' abc.csv

- display the first 2 rows in the up
* head -3 abc.csv

- display the last 2 rows in the bottom
* tail -2 abc.csv

- display the number of rows 
* wc -l abc.csv

- find the '24' data and display it
* head -n4 xyz.csv | grep '24'


**Author:** punya2001-pk 

::create csv file
[2021ict123@fedora ~]$ touch pqr.csv

::open file to edit it
[2021ict123@fedora ~]$ vi pqr.csv

::view the data in csv file
[2021ict123@fedora ~]$ more pqr.csv

![1](https://github.com/user-attachments/assets/f1779f1d-f848-4dca-a1f0-636886f62454)


::search "Engineering" in csv file
[2021ict123@fedora ~]$ grep 'Engineering' pqr.csv

![2](https://github.com/user-attachments/assets/c863ac9b-f6c3-4a25-9fb1-8aaf27a94316)



::display 5 rows in up to bottom in csv file
[2021ict123@fedora ~]$ head -5 pqr.csv

![3](https://github.com/user-attachments/assets/3ea1b9f2-2b0e-49d5-a278-7c5de1d445a2)


::display 3 rows in bottom to up in csv file
[2021ict123@fedora ~]$ tail -3 pqr.csv

![4](https://github.com/user-attachments/assets/43fa5a38-3589-439e-b031-a92d83787653)


::display number of columns
[2021ict123@fedora ~]$ awk -F, '{print NF;exit}' pqr.csv

![6](https://github.com/user-attachments/assets/1f09ec98-ed92-4153-95e2-4089c30fe8f6)


::display only age
[2021ict123@fedora ~]$ awk -F, '{print $3}' pqr.csv

![7](https://github.com/user-attachments/assets/e2a1e555-7c62-4d85-95f6-a1de3e141496)



::display 7th row 
[2021ict123@fedora ~]$ head -n7 pqr.csv | tail -n1

![8](https://github.com/user-attachments/assets/3cdf3848-04aa-4c93-9e4c-e279c079c666)



::display last 3 rows in csv file
[2021ict123@fedora ~]$ tail -3 pqr.csv

![9](https://github.com/user-attachments/assets/e9298abd-72ed-486c-b374-807c983d7b18)


::display salary
[2021ict123@fedora ~]$ cut -d, -f4 pqr.csv

![10](https://github.com/user-attachments/assets/45a85dcb-c016-473a-8039-b5eee2fb1920)


::display 2nd and 3rd columns
[2021ict123@fedora ~]$ awk -F, '{print $2 "," $3}' pqr.csv

![11](https://github.com/user-attachments/assets/60546499-2b72-429e-a65a-c3105331a082)


::display 2nd and 3rd columns and save a new file
[2021ict123@fedora ~]$ awk -F, '{print $2 "," $3}' pqr.csv > pqr2.csv
[2021ict123@fedora ~]$ more pqr2.csv

![12](https://github.com/user-attachments/assets/a72d1ed4-d4b9-41a4-847b-31b046399f74)


::display sort the salary 
[2021ict123@fedora ~]$ awk -F, '{print $4}' pqr.csv | sort

![13](https://github.com/user-attachments/assets/cae28c5c-ebb6-4751-a84f-b78384d76bef)


::sort the all csv data and display it
[2021ict123@fedora ~]$ sort -t',' -k4,4n pqr.csv

::display the order of the age (max to min)
[2021ict123@fedora ~]$ sort -t',' -k3,3nr pqr.csv

::display the order of the salary(max to min)
[2021ict123@fedora ~]$ sort -t',' -k4,4 -r pqr.csv


![14](https://github.com/user-attachments/assets/54467abb-d8b9-407d-9fa1-94f0ef000b27)


::display the 2nd and 4th columns sort by alperbaticaly order
[2021ict123@fedora ~]$ sort -t',' -k2,2 | sort -t',' -k4,4 -r pqr.csv

![15](https://github.com/user-attachments/assets/33dda023-e858-4f8a-ac99-1ff3086d1015)











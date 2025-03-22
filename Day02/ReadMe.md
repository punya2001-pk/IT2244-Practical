# ***** Pro1.txt *****

- First open the putty and enter the host name : 127.16.140.150 and press open button

- enter the registration number : 2021ict123

- enter the password : 789*asd
 [2021ict123@fedora~]$

- create new empty file
[2021ict123@fedora ~]$ touch abc.csv

- text editor
[2021ict123@fedora ~]$ vi abc.csv

- enter the data and press ctrl+c(save) -> shift+: -> wq!

- shown as content of the file
[2021ict123@fedora ~]$ more abc.csv
45,85,65,54
64,52,65,41
52,78,41,50

- display the number of rows
[2021ict123@fedora ~]$ wc -l abc.csv

- Extracts columns 1 and 3
[2021ict123@fedora ~]$ cut -d ',' -f 1,3 abc.csv

- Extracts columns 1 and 3 from abc.csv , display the output to a new file abc1.csv
[2021ict123@fedora ~]$ cut -d ',' -f 1,3 abc.csv > abc1.csv

- Displays the first 3 lines of the file abc.csv
[2021ict123@fedora ~]$ head -3 abc.csv

- Displays the last 2 lines of the file abc.csv
[2021ict123@fedora ~]$ tail -2 abc.csv


# ***** Pro2.txt *****

- enter the birthyear and get the age

@echo off 
set/p birthyear=Enter your birthyear:
set/a age=%date:~ 10,4% -%birthyear%
echo age:%age% yearold
pause

![Pro2](https://github.com/user-attachments/assets/a0200697-d37a-44b2-9fd4-492f2e3d8e8a)

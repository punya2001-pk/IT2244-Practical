Q1. write a code for small astrology based on your life path number for that get date of birth from user then calculate life path number.(use switch case)

example:

calculation for life path number:

	a=date%10
 
	b=date/10
 
	c=a+b
	
if life path number:

	1:Lucky
 
	2:Carefuly do your work
 
	3:Strange
 
	4:Happy
 
	5:Can get help
 
	6:Doubt
 
	7:sad
 
	8:Like
 
	9:Courage
	
CODE:	

echo "Enter the birth date: "

read date

a=$(($date%10))

b=$(($date/10))

c=$(($a+$b))

case $c in

        1)echo "Lucky";;
        
        2)echo "Carefuly do your work";;
        
        3)echo "Strange";;
        
        4)echo "Happy";;
        
        5)echo "Can get help";;
        
        6)echo "Doubt";;
        
        7)echo "sad";;
        
        8)echo "Like";;
        
        9)echo "Courage";;
esac

![1](https://github.com/user-attachments/assets/fefda58f-9e67-4cef-bfa9-5f2d4c9e577c)

![Screenshot 2025-04-11 150131](https://github.com/user-attachments/assets/98a47796-4c45-49e4-b3e1-cb9a5cd4444e)


.............................................................................................................................

Q2. Give list of numbers then calculate the summation and multiplication using for loop.
Example:
1	2	3	4	5
summation :15
multiplication :120

*********************************
syntax for For loop:            *
   for variable in list         * 
		do                  	      * 
		  commands          	      *
	done                          *
*********************************								
syntax for while loop:	        *
	while[condition]		        	*
		do			  			            *
		 commands		  		          *
	done				  		            *
								                *
*********************************

CODE:
sum=0
mul=1
for num in 1 2 3 4 5
do
sum=$(($sum+$num))
mul=$(($mul*$num))
done
echo "Summation:$sum"
echo "Multiplication:$mul"


![2](https://github.com/user-attachments/assets/c7204ac8-3b92-4274-b71f-a90ab85b5288)


.............................................................................................................................

Q3. Print the integers from 1 to 10 using while loop

CODE:
let 
while [ $i -le 10 ]
do
echo $i
i=$(($i+1))
done

![3](https://github.com/user-attachments/assets/37953607-764a-4266-ad4b-8fba25409600)


.............................................................................................................................

Q4. Print below pattern using nested loop
column 7 row 7

<img width="310" alt="q" src="https://github.com/user-attachments/assets/f9795db9-1ab5-47a7-8a5d-946694ef1840" />


CODE:

echo 'Enter number of Rows: '
read rows
echo 'Enter number of Columns: '
read cols

for ((i=1; i<=rows; i++))
do
for ((j=1; j<=i; j++))
do
echo -n '* '
done
echo ''
done

echo " "

for ((i=1; i<=rows; i++))
do
for ((j=cols+1; j>i; j--))
do
echo -n '* '
done
echo ''
done


![5](https://github.com/user-attachments/assets/37444884-0ed7-40b7-89fe-758199590e2b)


.........................................................................................................................

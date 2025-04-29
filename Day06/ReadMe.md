Q1. Get the calender and date

[2021ict123@fedora ~]$ cal
  
[2021ict123@fedora ~]$ date

![1](https://github.com/user-attachments/assets/a65dc311-b589-44f8-b826-9de13f124352)


...............................................................................................

Q2. Get the student name and marks for the 3 subjects from user then calculate
output:
Enter the name:Isuru
Enter the marks for subject1:85
Enter the marks for subject2:75
Enter the marks for subject3:80
Total = 240
Average = 80

echo "Enter the name: "
read name
echo "Enter the marks for subject1: "
read subject1
echo "Enter the marks for subject2: "
read subject2
echo "Enter the marks for subject3: "
read subject3
add=$(($subject1+$subject2+subject3))
echo "Total = " $add
average=$(($add/3))
echo "Average = " $average

![2](https://github.com/user-attachments/assets/c2ad96c4-8fa3-4e55-8096-3a559ac8f08b)


...............................................................................................

Q3. Create calculator with arithmetic operators

Enter the first number:4
Enter the second number:2
Summation:6
Division:2
Multiplication:8

echo "Enter the first number: "
read number1
echo "Enter the second number: "
read number2
sum=$(($number1+$number2))
echo "Summation: " $sum
div=$(($number1/$number2))
echo "Division: " $div
mul=$(($number1*$number2))
echo "Multiplication: " $mul


![3](https://github.com/user-attachments/assets/3d877ea2-68c2-456f-a3ab-50c14b3e67cf)


...............................................................................................

Q4. Get the days based on the user input number
output:
Enter the number:5
friday

echo "Enter the number: "
read num
case $num in
  1) echo "Monday" ;;
  2) echo "Tuesday" ;;
  3) echo "Wednesday" ;;
  4) echo "Thursday" ;;
  5) echo "Friday" ;;
  6) echo "Saturday" ;;
  7) echo "Sunday" ;;
  *) echo "Invalid input! Please enter a number between 1 and 7." ;;
esac

![4](https://github.com/user-attachments/assets/7ba5dfda-e16d-4f32-8aff-3e60ebd0a56e)


...............................................................................................

Q5. verify whether your user name is correct or not.(Use your name as a)
output:
Enter user name:
Mino
User name is correct
Enter user name:
Mino
User name is incorrect


username="Mino"
echo "Enter the user name:"
read name

if [[ "$username" != "$name" ]]; then
    echo "User name is incorrect"
else
    echo "User name is correct"
fi


![5](https://github.com/user-attachments/assets/50b10b1a-f731-424a-8bae-a99847df0cce)


...............................................................................................

Q6. enter two numbers and display the greater than number and less than number
output:
Enter two numbers:
7   5
7 is greater than 5

Enter two numbers:
1   9
1 is less than 9


echo "Enter two numbers:"
read num1
read num2

if [ "$num1" -gt "$num2" ]; then
    echo "$num1 is greater than $num2"
else
    echo "$num2 is greater than $num1"
fi

if [ "$num1" -lt "$num2" ]; then
    echo "$num1 is less than $num2"
else
    echo "$num2 is less than $num1"
fi

![6](https://github.com/user-attachments/assets/7acaff69-fbbd-4ce7-9462-b3bd4f2f7353)

![7](https://github.com/user-attachments/assets/0f6e81eb-af04-40ca-a826-419c3b015d3b)


...............................................................................................

Q7. create simple calculator using "expr" command same as the Q3

echo "Enter the name: "
read name
echo "Enter the marks for subject1: "
read subject1
echo "Enter the marks for subject2: "
read subject2
echo "Enter the marks for subject3: "
read subject3
add=$(($subject1+$subject2+subject3))
echo "Total = " $add
add='expr $subject1+$subject2'

![8](https://github.com/user-attachments/assets/4ace6d4f-1a30-4b4b-bde6-757b4d14cfc9)


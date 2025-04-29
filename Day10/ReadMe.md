## Que01:

Print multiplication table using for loop

	1 * 2 = 2
 
	2 * 2 = 4
 
	.......
	
Code:

[2021ict123@fedora ~]$ touch Que1.sh

[2021ict123@fedora ~]$ vi Que1.sh

echo "Enter the number: "

read num

for((i=1;i<=12;i++))

do

mul=$(($i*$num))

echo "$i*$num=$mul"

done	

![Q1](https://github.com/user-attachments/assets/6027ad10-13fc-4ed9-8d68-8142629f81dc)

.............................................................................................................................

## Que02: 

 <img width="184" alt="q" src="https://github.com/user-attachments/assets/761a7cf7-dea9-468d-803c-9a4e75a2343d" />


Code:

[2021ict123@fedora ~]$ vi q2.sh

echo 'Enter number of Rows: '

read rows

## Top half of the diamond

for ((i=1; i<=rows; i++))

do

    for ((k=i; k<rows; k++))
    
    do
    
        echo -n " "
	
    done

    for ((j=1; j<=((2*i-1)); j++))
    
    do
    
        echo -n "*"
	
    done
    
    echo 
    
done

## Bottom half of the diamond

for ((i=rows-1; i>=1; i--))

do

    for ((k=rows; k>i; k--))
    
    do
    
        echo -n " "
	
    done

    for ((j=1; j<=((2*i-1)); j++))

    do
    
        echo -n "*"
	
    done

    echo ""
done

![Q2](https://github.com/user-attachments/assets/178dc9ca-a401-4c59-842e-6fdcae3c5da7)


.............................................................................................................................
 
## Que03: 
 
Fibonacci Series:

0 1 1 2 3 5 8 13 21 34

Sum of the first 10 Fibonacci numbers is: 88
 
Code:

a=0

b=1

sum=1  

echo -n "Fibonacci Series: "

echo -n "$a $b "

for ((i=3; i<=10; i++))

do

    fib=$((a + b))
    
    echo -n "$fib "
    
    sum=$((sum + fib))
    
    a=$b
    
    b=$fib
    
done

echo ""

echo "Sum of the first 10 Fibonacci numbers is: $((sum + 0))"

<img width="363" alt="Q3" src="https://github.com/user-attachments/assets/7e9a1c73-2ed0-4f4c-8487-962e3253f3a4" />


.............................................................................................................................

## Que04:

Sum of prime numbers between 1 and 100 is:1060

echo ""  

sum=0   

for ((num=2; num<=100; num++)) 

do

    is_prime=1  
    
    for ((i=2; i<=num/2; i++)) 
    
    do
    
        if ((num % i == 0)); then 
	
            is_prime=0
	    
            break
	    
        fi
	
    done

    if ((is_prime == 1)); then  
    
        sum=$((sum + num))
    fi
    
done

echo "Sum of prime numbers between 1 and 100 is: $sum"

 <img width="413" alt="Q4" src="https://github.com/user-attachments/assets/b00682e1-72ca-46fb-ac2e-7d1824593543" />

 
.............................................................................................................................
 


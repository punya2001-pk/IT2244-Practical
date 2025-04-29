
## Q1) Fibbonacci series: (Output: First 10 fibbonacci numbers: 0 1 1 2 3 5 8  13 21 34)

CODE:

echo ""

echo "....Fibonacci...."

base1=0

base2=1

echo -n "$base1 $base2 "

for((a=2; a<=10; a++))

do

Fibo=$(($base1+$base2))

echo -n "$Fibo "

base1=$base2

base2=$Fibo

done

![2](https://github.com/user-attachments/assets/bf09dd91-9bea-4519-b8f2-d5736d9c9752)


## Q2) Factorial(Output: Factorial of 5 is: 120)

CODE:

echo "Enter the number: "

read number

fact=1

for((i=1;i<=number;i++))

do

fact=$(($fact*$i))

done

echo "Factorial of number:$fact"

![1](https://github.com/user-attachments/assets/cec802a1-067c-4264-a52f-3cb5d089d70a)


## Q3) Multiples of 3 between 1 and 50

CODE:

echo ""

echo "....Multiples of 3...."

number=3

for(( a=1; a<=16; a++))

do

mul=$(($number*$a))

echo -n "$mul "

done

for((a=3; a<50; a+=3))

do

echo -n "$a"

done

![3](https://github.com/user-attachments/assets/5ae030dd-ecb6-4204-8edc-d1e2ab662c68)


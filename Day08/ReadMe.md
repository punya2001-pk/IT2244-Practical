#Display this patterns

<img width="248" alt="q" src="https://github.com/user-attachments/assets/2dbe5c96-953f-4b68-9c5f-4b3fc1d85d8d" />


CODE:

echo 'Enter number of Rows: '
read rows
echo 'Enter number of Columns: '
read cols


for ((i=1; i<=rows; i++))
do
for ((j=1; j<=i; j++))
do
echo -n $i " "
done
echo ''
done

echo " "

for ((i=1; i<=rows; i++))
do
for ((j=1; j<=i; j++))
do
echo -n $j " "
done
echo ''
done

echo " "

for ((i=1; i<=rows; i++))
do
    for ((k=1; k<=rows-i; k++))
    do
        echo -n " "
    done

    for ((j=1; j<=i; j++))
    do
        echo -n "* "
    done

    echo ""
done

![Screenshot (69)](https://github.com/user-attachments/assets/6ab79a1f-f61d-4fee-83d6-94a248e65900)


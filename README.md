# Recursive-function

## Aim:
To write a C# program to reverse a number using recursive function.

## Algorithm:
## Step1:
Create a function for reversing.

## Step2:
Get the number from the user.

## Step3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

## Step4:
Recusively call this function to get the reversed number.

## Step5:
print the reversed number.
## Program:
```python
using System;

namespace exp7
{
    class Program
    {
        int rem = 0, rev = 0;
        public int reverse(int n)
        {
            rem = n % 10;
            if (rem == 0) return rev;
            else
            {
                rev = rev * 10 + rem;
                return reverse(n / 10);
            }
        }
        static void Main(string[] args)
        {
            int n;
            Console.WriteLine("Enter a Number to reverse: ");
            n = Convert.ToInt32(Console.ReadLine());

            Program p1 = new Program();
            Console.WriteLine("Reversed Number is "+ p1.reverse(n));
        }
    }
}
```
## Output:

![Screenshot 2022-06-20 012320](https://user-images.githubusercontent.com/75235233/175008941-ddd494d5-b663-404a-8534-9b2af7c7edb0.png)



## Result:
Thus C# program to reverse a number using recursive function is written and executed sucessfully.

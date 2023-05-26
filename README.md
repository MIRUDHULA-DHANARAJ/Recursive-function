# Recursive-function

## Aim:
To write a C# program to reverse a number using recursive function.

## Algorithm:

## Step 1:
Create a function for reversing.

## Step 2:
Get the input from the user.

## Step 3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

## Step 4:
Recursively calling the function to get the reversed number.

## Step 5:
Print the reversed number.

## Program:
```
Developed By: Mirudhula D
Register no.: 212221230060
```
```
using System;
namespace hello
{
    class program
    {
        int rev = 0, rem;
        public int reverse(int n)
        {
            rem = n % 10;
            if (rem == 0)
            {
                return rev;
            }
            else
            {
                rem = n % 10;
                rev = rev * 10 + rem;
                n = n / 10;
                return reverse(n);
            }
        }
    }
    class name
    {
        static void Main(string[] args)
        {
            int n;
            Console.Write("Enter number to be reversed: ");
            n = Convert.ToInt32(Console.ReadLine());

            program p = new program();
            Console.WriteLine("The reversed number is : " + p.reverse(n));
        }
    }
}
```

## Output:

![EXP-7](https://github.com/MIRUDHULA-DHANARAJ/Recursive-function/assets/94828147/9d723327-bd46-4ca5-819f-1d3a5fcd82f8)


## Result:

Thus, a C# program to reverse a number using recursive function is executed successfully.

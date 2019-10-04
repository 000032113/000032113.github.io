---
layout: post
title: Money Conversions
catagories: C#
---

# Task
The task was to create a program that will allow a user to convert from pounds to dollars ance vice versa. This inculded creating
varaibles, constants and switch case.

# Method
## Step 1
I began by declaring the constants for the rate of conversions:
```csharp
double PoundToDollar = 1.67;
double DollarToPound = 0.59;
```
Constants are similar to variables, but they cannot be changed while the program is being run.
## Step 2
I then got the user to enter a value for the price they wanted to be converted:
```csharp
Console.WriteLine("Enter value:");
double ConvertValue = Convert.ToDouble(Console.ReadLine());
```
I had to convert the value to a double, so that decimal values could be entered.
## Step 3
The last step was using switch case, which allowed to user to choose what currency they wanted to convert to:
```csharp
Console.WriteLine("Enter 1 for Pounds to Dollar \nEnter 2 for Dollar to Pounds");
int option = Convert.ToInt16(Console.ReadLine());
switch (option)
{
case 1:
Console.WriteLine("£" + ConvertValue + " to Dollars is $" + Math.Round(ConvertValue * PoundToDollar,2));
Console.ReadLine();
break;
case 2:
Console.WriteLine("$" + ConvertValue + " to Pounds is £" + Math.Round(ConvertValue * DollarToPound,2));
Console.ReadLine();
break;
default:
break;
}
```
During this I used the Math.Round function to round the resulting value to 2 decimal places, because that is how money is presented.

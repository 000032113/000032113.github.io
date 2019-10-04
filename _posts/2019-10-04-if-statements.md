---
layout: post
title: If statements
catagories: C#
---

# Task 1
The task was to create a program that asks the user for 3 numbers and writes "SNAP" if all three are the same ortherwise it should write
"No match".
# Method
## Step 1
I began by asking the user for 3 numbers. I did this by using the Console.WriteLine and Console.ReadLine functions:
```C#
Console.WriteLine("Enter first number");
int a = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Enter second number");
int b = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Enter third number");
int c = Convert.ToInt32(Console.ReadLine());
```
I also needed to cast each variable into integers, as numbers were being entered.
## Step 2
I then had to continue with an If statement to decide whether the number were equal to eachother:
```C#
if (a == b && b == c)
{
Console.WriteLine("SNAP");
Console.ReadLine();
}
else
{
Console.WriteLine("No match");
Console.ReadLine();
}
```
During this I also had to use the AND comparison, which in C# is &&.
# Task 2
The task was to ask the user for a mark and convert it into what grade it is worth.
# Method
## Step 1
I started by declaring the variables score and grade, casting them into and integer and a character:
```C#
Console.WriteLine("Enter score");
int score = Convert.ToInt32(Console.ReadLine());
char grade = ' ';
```
I also had to convert the user input into and integer so calculations could be performed.
## Step 2
I then had to include an If Statement to decide what grade the score fell under, assigning the variable grade a new value depending on
what grade they achieved:
```C#
if (score < 40)
{
grade = 'U';
}
else if (score < 50)
{
grade = 'D';
}
else if (score <60)
{
grade = 'C';
}
else if (score < 70)
{
grade = 'B';
}
else
{
grade = 'A';
}
Console.WriteLine("Your grade is " + grade);
Console.ReadLine();
```
I used the Console.WriteLine function to then print what grade was achieved.

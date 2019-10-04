---
layout: post
title: calculations
categories: C#
---

# Task
The task was to find the volume and surface area of a cylinder.
# Method
## Step 1
I started off by declaring the constant PI, and having the user enter the necessary measurements:
```csharp
const double PI = 3.1415926535897932384;
Console.WriteLine("Enter Radius of cylinder in cm");
double r = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("Enter height of cylinder in cm");
double h = Convert.ToDouble(Console.ReadLine());
```
## Step 2
I then performed the calculations, with the operation *:
```C#
Console.WriteLine("Volume = " + Math.Round(PI*r*r*h,2));
double sa = Math.Round((2 * PI * r * r) + (2 * PI * r * h),2);
Console.WriteLine("Surface Area = " + sa);
Console.ReadLine();
```
I also rounded to 2 decimal places using the Math.Round funstion.

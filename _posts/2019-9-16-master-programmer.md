---
layout: post
title: master programmer
categories: C#
---

## I have programmed some cool stuff today :D

```csharp
const double PI = 3.1415926535897932384;
Console.WriteLine("Enter Radius of cylinder in cm");
double r = Convert.ToDouble(Console.ReadLine());Console.WriteLine("Enter height of cylinder in cm");
double h = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("Volume = " + Math.Round(PI*r*r*h,2));
double sa = Math.Round((2 * PI * r * r) + (2 * PI * r * h),2);
Console.WriteLine("Surface Area = " + sa);
Console.ReadLine();
```
### This program finds the volume and surface area of a cylinder

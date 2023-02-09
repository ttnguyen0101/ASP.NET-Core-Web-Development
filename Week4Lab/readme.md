# Week 4 Lab
## Test and Debug 
In this lab, I learned to test and debug an ASP.NET Core MVC web app using the Error List Window, Internal Server Error page, breakpoint, and browser's Developer Tools.

Here is the list of all errors, both syntax and logic, found in the Tip Calculator app and what change was made to fix them:
- site.css: change `widht` to `width`
- _Layout.cshtml: missing opening tag of `<html>` → add opening tag for `<html>` on line 2
- TipCalculator.cs: line 16, missing `;` after return statement → add `;` 
- HomeController.cs: line 14, `Viewbag` with "b" in lower case → change `Viewbag` to `ViewBag`
- HomeController.cs: function missing return value → add `return` in front of `View()` on line 17
- Index.cshtml: line 16, change `Fifteem` to `Fifteen`
- TipCalculator.cs: line 15 has wrong logic, tip calculation should be multiplying meal cost to tip percent instead of dividing → change `MealCost.Value / percent` to `MealCost.Value * percent`

# CSS `calc()` Miscalculation with Percentages

This repository demonstrates a common yet subtle issue with the CSS `calc()` function when dealing with percentage values. The issue arises when combining percentages with addition or subtraction, leading to unexpected results in some scenarios.

## Problem
The root cause of this issue lies in the order of operations within the `calc()` function. Percentages are resolved before arithmetic operations. This can lead to incorrect calculations, especially when the percentages are dependent on the size of their parent elements.

## Solution
To address this, restructure your CSS to avoid relying on percentage calculations directly inside `calc()`. One approach is to use a combination of `em`, `rem`, or `vw` units along with the percentage values.
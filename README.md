# R Bug: Handling NA values in mean calculation

This repository demonstrates a common error in R programming related to handling `NA` values when calculating the mean of a numeric vector. The `bug.R` file contains code that produces an unexpected result because it doesn't handle the presence of `NA` values. The `bugSolution.R` file provides a corrected version that demonstrates proper `NA` handling.

The issue is that the `mean()` function in R returns `NA` if any `NA` values are present in the input vector.  This behavior can be problematic when dealing with real-world data that often contains missing values. The solution demonstrates two common methods to deal with this problem: removing NAs before applying mean and using the `na.rm` argument.
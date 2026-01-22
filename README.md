
## Function

_multlinreg("y", ["x1", "x2", "x3", ... "xn"], "datafile.csv")_

multlinreg is used to run multiple linear regression, given user-specified outcome and any number of predictors from a .csv file. It is dependent on the following libraries: NumPy, Pandas, scipy.stats, and os. This function using only ordinary least squares and linear algebra, without the use of existing regression functions.

## Function Inputs

"y": the outcome variable. This is the variable that we are associating with the x variables.

["x1", "x2", ... "xn"]: the predictor variable(s). This may be any number of variables. All predictor variables must be separated by commas, individually within quotations, and collectively contained within brackets.

"datafile.csv": data file. Must be csv file (See errors below). The function includes a read_csv function, so previously reading the file is not required (but recommended).

## Function Outputs

Parameter estimates for all predictors (including intercept)

Standard error for all predictors

t-statistic for all predictors

Two-tailed p-value for all predictors

R-squared goodness of fit measure

Adjusted R-squared

F-statistic and degrees of freedom, and corresponding p-value

## Errors

"ERROR: FILE MUST BE .CSV.": The given file type in the third argument of the function is not a .csv file.

"ERROR: Variable(s) {x1, x2} were not found in {datafile}": Given output or predictor variable names are not found in the specified data file. Variables that were not found are specified within the error message.

Other cases: If there is missing data in the .csv file, the output will result in NA values.

Examples at the end of document

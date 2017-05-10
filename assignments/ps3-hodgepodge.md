Problem set \#3: Regression diagnostics, interaction terms, and missing data
================
MACS 30200 - Perspectives on Computational Research
**Due Monday March 15th at 11:30am**

-   [Regression diagnostics (5 pts)](#regression-diagnostics-5-pts)
-   [Interaction terms (5 pts)](#interaction-terms-5-pts)
-   [Missing data (5 pts)](#missing-data-5-pts)
-   [Submission instructions](#submission-instructions)
    -   [If you use R](#if-you-use-r)
    -   [If you use Python](#if-you-use-python)

![](https://s3.amazonaws.com/media.thecrimson.com/photos/2014/10/02/103651_1299339.jpg)

Regression diagnostics (5 pts)
==============================

Estimate the following linear regression model of attitudes towards Joseph Biden:

*Y* = *β*<sub>0</sub> + *β*<sub>1</sub>*X*<sub>1</sub> + *β*<sub>2</sub>*X*<sub>2</sub> + *β*<sub>3</sub>*X*<sub>3</sub>

where *Y* is the Joe Biden feeling thermometer, *X*<sub>1</sub> is age, *X*<sub>2</sub> is gender, and *X*<sub>3</sub> is education. Report the parameters and standard errors.

> For this section, be sure to `na.omit()` the data frame (listwise deletion) before estimating the regression model. Otherwise you will get a plethora of errors for the diagnostic tests.

1.  Test the model to identify any unusual and/or influential observations. Identify how you would treat these observations moving forward with this research. Note you do not actually have to estimate a new model, just explain what you would do. This could include things like dropping observations, respecifying the model, or collecting additional variables to control for this influential effect.
2.  Test for non-normally distributed errors. If they are not normally distributed, propose how to correct for them.
3.  Test for heteroscedasticity in the model. If present, explain what impact this could have on inference.
4.  Test for multicollinearity. If present, propose if/how to solve the problem.

Interaction terms (5 pts)
=========================

Estimate the following linear regression model:

*Y* = *β*<sub>0</sub> + *β*<sub>1</sub>*X*<sub>1</sub> + *β*<sub>2</sub>*X*<sub>2</sub> + *β*<sub>3</sub>*X*<sub>1</sub>*X*<sub>2</sub>

where *Y* is the Joe Biden feeling thermometer, *X*<sub>1</sub> is age, and *X*<sub>2</sub> is education. Report the parameters and standard errors.

> Again, employ listwise deletion in this section prior to estimating the regression model.

1.  Evaluate the marginal effect of age on Joe Biden thermometer rating, conditional on education. Consider the magnitude and direction of the marginal effect, as well as its statistical significance.
2.  Evaluate the marginal effect of education on Joe Biden thermometer rating, conditional on age. Consider the magnitude and direction of the marginal effect, as well as its statistical significance.

Missing data (5 pts)
====================

Estimate the following linear regression model of attitudes towards Joseph Biden:

*Y* = *β*<sub>0</sub> + *β*<sub>1</sub>*X*<sub>1</sub> + *β*<sub>2</sub>*X*<sub>2</sub> + *β*<sub>3</sub>*X*<sub>3</sub>

where *Y* is the Joe Biden feeling thermometer, *X*<sub>1</sub> is age, *X*<sub>2</sub> is gender, and *X*<sub>3</sub> is education. This time, use multiple imputation to account for the missingness in the data. Consider the multivariate normality assumption and transform any variables as you see fit for the imputation stage. Calculate appropriate estimates of the parameters and the standard errors and explain how the results differ from the original, non-imputed model.

Submission instructions
=======================

Submit your work in the `PS3` folder in your project repo.

If you use R
------------

Submit your assignment as a single [R Markdown document](http://rmarkdown.rstudio.com/). R Markdown is similar to Juptyer Notebooks and compiles all your code, output, and written analysis in a single reproducible file.

If you use Python
-----------------

Either:

1.  Submit your assignment following the same procedures as required by Dr. Evans. Submit a Python script containing all your code, plus a LaTeX generated PDF document with your results and substantive analysis.
2.  Submit your assignment as a single Jupyter Notebook with your code, output, and written analysis compiled there.

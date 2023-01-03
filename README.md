# STATISTICAL-ANALYSIS-YSING-SAS-9.4-SOFTWARE
ANALYSING AND STATISTICAL TESTING OF DATA

# ABOUT THE PROJECT

This repository is about the statistical analysis that is done in SASsoftware to test is their is any significant difference in the serum lipid peroxide between the treatment andcontrol group.The data should include two variables that will be used in the analysis. The independent variable is undergoing treatment and the dependent variable is the serum lipid peroxide level.

# STATISTICAL ANALYSIS

Statistical Analysis is done by using SAS 9.4 Software, To test the statistical significance in the serum ipid peroxide between the two groups.Independent t test is used for the analysis to compare the mean of serum lipid peroxide level after analysing the normality of the data.
*representation of data is done by using pie chart and histogram.
*descriptive statistics ofthe data is also calculated.
*normality of the data is also checked.
H0:  There is no significant difference in the mean level of serum lipid peroxide between the treatment and control group.
H1:  There is a significant difference in the mean level of serum lipid peroxide between the treatment and control group.

# goal
 
 Performing an appropriate test at 95% confidence to compare the serum lipid peroxide level between the subjects who were undrgoing treatment for diabettis mellittus and healthy controls.
 
 # result
 
 The pvalue of pooled variance is greater than 0.05 so we failed to reject the null hypothesis at 95% confidence that is thereis no significant difference in the mean level of serum lipid peroxide between the treatment and control group.
 
 # PROGRAM
 
 
 
 
 
 
 
 
 
 
 
 # CHART[A   STATISTICAL  ANALYSIS  USING SAS.docx](https://github.com/ANSU481/STATISTICAL-ANALYSIS-YSING-SAS-9.4-SOFTWARE/files/10337917/A.STATISTICAL.ANALYSIS.USING.SAS.docx)
[A   STATISTICAL  ANALYSIS  USING SAS.docx](https://github.com/ANSU481/STATISTICAL-ANALYSIS-YSING-SAS-9.4-SOFTWARE/files/10337924/A.STATISTICAL.ANALYSIS.USING.SAS.docx)

 
 
 PROC GCHART DATA=WORK.IMPORT;
 PIE3D GROUP;
 RUN;
 PROC GCHART UNIVARIATE DATA=WORK.IMPORT;
 HISOGRAM AGE;
 RUN;
 
 #DESCRIPTIVE STATISTICS
 
  PROC UNIVARIATE DATA=WORK.IMPORT;
  VAR SLPLEVEL;
  CLASS GROUP;
  RUN;
  
  #NORMALITY
  
  PROC UNIVARIATE DATA=WORK.IMPORT NORMAL;
  VAR SLPLEVEL;
  CLASS GROUP;
  RUN;
  
  #TTEST
  
  PROC TTEST DATA=WORK.IMPORT;
  VAR SLPLEVEL;
  CLASS GROUP;
  TITLE"INDEPENDENT TWO SAMPLE T TEST "[A   STATISTICAL  ANALYSIS  USING SAS.docx](https://github.com/ANSU481/STATISTICAL-ANALYSIS-YSING-SAS-9.4-SOFTWARE/files/10337935/A.STATISTICAL.ANALYSIS.USING.SAS.docx)

  RUN;
  
  
 
 



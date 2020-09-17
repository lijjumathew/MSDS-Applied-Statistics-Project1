# Stats2Project1


## From the Full Model the below are the significant predictors - Forward Selection


Adult.Mortality                 -1.730e-02  4.586e-03  -3.772 0.000263 ***
infant.deaths                    3.647e-01  1.102e-01   3.309 0.001270 ** 
Alcohol                          1.928e-01  9.368e-02   2.058 0.041997 *  
under.five.deaths               -2.948e-01  8.244e-02  -3.576 0.000521 ***
HIV.AIDS                        -5.697e-01  2.959e-01  -1.926 0.056758 .  
Income.composition.of.resources  3.141e+01  5.572e+00   5.638 1.37e-07 ***

Residual standard error: 3.323 on 109 degrees of freedom
Multiple R-squared:  0.8817,	Adjusted R-squared:  0.8622 
AIC=690.1365  BIC=747.1771
ASE=9.405684

## From the Full Model the below are the significant predictors - Backward Selection


Adult.Mortality                 -0.019037   0.004314  -4.413 2.24e-05 ***
infant.deaths                    0.346787   0.091338   3.797 0.000231 ***
Alcohol                          0.190732   0.084952   2.245 0.026588 *  
under.five.deaths               -0.278161   0.072770  -3.822 0.000211 ***
Total.expenditure                0.208568   0.106121   1.965 0.051680 .  
HIV.AIDS                        -0.542359   0.271797  -1.995 0.048258 *  
Income.composition.of.resources 32.084721   3.092474  10.375  < 2e-16 ***

Residual standard error: 3.238 on 120 degrees of freedom
Multiple R-squared:  0.8764,	Adjusted R-squared:  0.8692  
AIC=673.8125  BIC=699.4808
ASE=9.832157

## From the Full Model the below are the significant predictors - Stepwise Selection


Adult.Mortality                 -0.019037   0.004314  -4.413 2.24e-05 ***
infant.deaths                    0.346787   0.091338   3.797 0.000231 ***
Alcohol                          0.190732   0.084952   2.245 0.026588 *  
under.five.deaths               -0.278161   0.072770  -3.822 0.000211 ***
Total.expenditure                0.208568   0.106121   1.965 0.051680 .  
HIV.AIDS                        -0.542359   0.271797  -1.995 0.048258 *  
Income.composition.of.resources 32.084721   3.092474  10.375  < 2e-16 ***

Residual standard error: 3.238 on 120 degrees of freedom
Multiple R-squared:  0.8764,	Adjusted R-squared:  0.8692
AIC=673.8125  BIC=699.4808
ASE=9.832157


## From the Reduced Model (stepwise selection) the below are the significant predictors 


Adult.Mortality                 -0.019037   0.004314  -4.413 2.24e-05 ***
infant.deaths                    0.346787   0.091338   3.797 0.000231 ***
Alcohol                          0.190732   0.084952   2.245 0.026588 *  
under.five.deaths               -0.278161   0.072770  -3.822 0.000211 ***
Total.expenditure                0.208568   0.106121   1.965 0.051680 .  
HIV.AIDS                        -0.542359   0.271797  -1.995 0.048258 *  
Income.composition.of.resources 32.084721   3.092474  10.375  < 2e-16 ***

Residual standard error: 3.238 on 120 degrees of freedom
Multiple R-squared:  0.8764,	Adjusted R-squared:  0.8692 
correlation        RMSE 
     0.7630      0.4363 
VIF
Adult.Mortality - 2.823806 
infant.deaths - 800.207011
Alcohol - 1.497704
under.five.deaths - 805.376827
Total.expenditure - 1.116503 
HIV.AIDS - 1.811741
Income.composition.of.resources - 2.760631
AIC=673.8125  BIC=699.4808
ASE=9.832157



## Lasso Predictors run with all Predictors

Adult.Mortality                 -0.0191246691
Alcohol                          0.1290622227
Total.expenditure                0.0559652197
Diphtheria                       0.0002095938
HIV.AIDS                        -0.4152214620
thinness..1.19.years            -0.0494267615
Income.composition.of.resources 34.2057499766



## From the Reduced Model (lasso selection) the below are the significant predictors 


Adult.Mortality                 -0.019658   0.004567  -4.305 3.43e-05 ***
Alcohol                          0.190417   0.089385   2.130   0.0352 *  
Total.expenditure                0.158346   0.114060   1.388   0.1676    
Diphtheria                       0.014960   0.014128   1.059   0.2918    
HIV.AIDS                        -0.631963   0.284766  -2.219   0.0284 *  
thinness..1.19.years            -0.112665   0.096625  -1.166   0.2459    
Income.composition.of.resources 33.338972   3.397006   9.814  < 2e-16 ***

Residual standard error: 3.402 on 120 degrees of freedom
Multiple R-squared:  0.8636,	Adjusted R-squared:  0.8556 
correlation        RMSE 
     0.8026      0.2577
VIF
Adult.Mortality - 2.867694 
Alcohol - 1.502603
Total.expenditure - 1.168843 
Diphtheria - 1.149265
HIV.AIDS - 1.802256
thinness..1.19.years - 1.544284
Income.composition.of.resources - 3.018706
AIC=686.4176  BIC=712.0859
ASE=10.8496




## From the Linear model Life Expectancy for Developing vs Developed

(Intercept)        81.138      1.298  62.493  < 2e-16 ***
StatusDeveloping  -11.636      1.429  -8.141 6.17e-14 ***

1. The P value of dummy variable StatusDeveloping is very significant suggesting that 
  there is statistical evidence of difference in average life expectancy between developing and developed countries.
2. The average life expectancy in developed countries is estimated to be 81.138
3. The average life expectancy in developing countries is 11.638 years less than developed countries.

## Final Models

Life.expectancy ~ Adult.Mortality +  Total.expenditure +  Income.composition.of.resources
Life.expectancy ~ Adult.Mortality +  Alcohol + Total.expenditure + HIV.AIDS + Income.composition.of.resources + thinness..1.19.years

                                                     
                     
# stock-analysis
## Overview of the Project

The overview of the project defines the purpose and background of this analysis.

###Background

Steve wants to expand the dataset he is analyzing to include the entire stock marker over the last few years. Therefore, the initial code provided to him needs to be refactored to remain efficient when processing thousands of stock trades to minimize processing time. 

### Purpose
The purpose of this project is to refactor the intial code provided to Steve, so that it can process thousands of trades efficiently.

##Results

The results provided here have a limitation. Although close, the return outputs of the refactored code are slightly different from the original code. This is due to an error in the code where the closing prices of each ticker are not successfully writing to the Ending Prices array. However, the net positive or negative return are comparable which makes the overall analysis below accurate. 

### Performance of the tickers, 2017 vs. 2018

As shown in the images below, the stock market returns in 2017 were higher than those of 2018. Eleven stocks delivered positive returns in 2017, while only 2 stocks delivered positive returns in 2018. 

![VBA_Challenge_2017](https://user-images.githubusercontent.com/82396931/117605995-37e3b980-b116-11eb-8722-cd2a436dfd26.png)
![VBA_Challenge_2018](https://user-images.githubusercontent.com/82396931/117606008-3a461380-b116-11eb-8e5a-72351ea869d7.png)

### Improvement in Execution Time

The refactored code compiled in 0.125 seconds for both 2017 and 2018, which is a significant improvement from the original execution time of 0.496 seconds for the 2017 worksheet and 0.484 seconds for he 2018 worksheet. The refactored code is approximately 4x faster in execution time.

## Summary Statement

The purpose of refactoring code is to improve the design of the code. There are several advantages to refactoring code, which include: removal of duplicate code, redesigning code to reduce the number of hardcoded lines and reducing run time while maintaining results quality. The refactoring process also allows programmers to improve documentation and readability of the code. However, it is important to be cognizant of the disadvantages of refactoring code, which include: possibility to introduce bugs, risk of overshooting deadlines, and faulty or suboptimal logic that lead to lower quality results. To avoid the disadvantages of refactoring code, it is recommended that the programming team have sufficient time to refactor and test the code thoroughly prior to the delivery deadline.

In this project, refactoring the code produced the following advantages: 
* the execution time is 4x faster
* the refactored code is easier to scale compared to the original code making it more agile for future development (i.e. if more tickers are added)
* the refactored code can be easily modified to expand the scope of the analysis provided (i.e. if Steve wants to process more data for each ticker)


However, in this project refactoring the code also lead to a notable disadvantage, where the uality of the "Return" calculation has dropped, not providing the exact results of the original script. While the overall analysis was congruent with the analysis from the results of the original code, in this case, the "returns" calculations cannot be relied upon for precise data. This disadvantage can be overcome with more development time.

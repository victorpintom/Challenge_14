# Challenge_14
## Machine Learning Trading Bot
### Challenge results found in https://github.com/victorpintom/Challenge_14.git 
## As a financial advisor for a top algo-trading financial advisory firm I seek to improve the existing algo trading system
### 1st iteration: By using a 4/100 short/long window on a dataset trained on a 3-month period basis, the trading algo shows higher strategy returns over those actuals as shown below:
## Tuning the baseline
### 1. Adjust size of training dataset. Original training dataset of 3 months was reduced to 1 month and then increased to 6 months. What impact resulted from increasing or decreasing the training window? - By reducing the training dataset to one month of data, the strategy returns were closer than the actual results. By incresing the training dataset to six months of data, the strategy returns were markedly higher than the actual results. As a conclusion, the larger the sample training dataset, the better the algo machine behaves in prividing higher than actual returns. 

![Iteration_1_3m](https://github.com/victorpintom/Challenge_14/assets/142464833/5664e9d1-e310-4070-8455-3dce8a337e57)

![Iteration_2_1m](https://github.com/victorpintom/Challenge_14/assets/142464833/b2dff62f-7dd2-48d9-b251-27e26ffc2736)

![Iteration_3_6m](https://github.com/victorpintom/Challenge_14/assets/142464833/80e1c002-7e57-4e16-b138-c376a844b6b3)


### 2. Adjust SMA inputs. Orginal SMA values of 4 and 100 were reduced to 2 and 50 and then increased to 8 and 200. What impact resulted from increasing or decreasing either or both of the SMA windows? - By reducing the SMA values to 2 and 50, there was no major impact on the algo strategy returns. By increasing the SMA values to 8 and 200, there was a significant impact as the strategy returns were lower than the actual returns. As a conclusion, the algo works better on shorter time frames, i.e. taking short term signals. such as 2/50 or 4/100.

![Iteration_1_3m_2_50](https://github.com/victorpintom/Challenge_14/assets/142464833/4738d511-964a-48ee-b36c-44eb0bfc4bc3)

![Iteration_1_3m_8_200](https://github.com/victorpintom/Challenge_14/assets/142464833/b78d1660-7453-4639-a67d-a70424eb6952)

### 3. Choose the set of parameters that best improved the trading algorithm returns - after different iterations, I conclude that the best combination is 6 months training data with a short/long SMA of 4 and 100.

![Iteration_4_6m_4_100](https://github.com/victorpintom/Challenge_14/assets/142464833/8532865d-3f8a-474f-8ccc-2cbcefc628d1)


## Evaluation Report
### As initially proposed (i.e. 3 months of training data and 4 / 100 SMA), the algo works OK. There are improvements that can be made by increasing the timeframe of the training dataset to 6 months. Further, the model can be improved even more by a classifier model. In my case, I used AdaBoost and the results show a better strategy return above the actual return.  

![Iteration_5_ADA](https://github.com/victorpintom/Challenge_14/assets/142464833/304bf690-3708-4323-8612-5e2a1edf1557)

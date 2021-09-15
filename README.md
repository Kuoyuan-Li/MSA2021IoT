# MSA2021IoT
This repository is dedicated for MSA 2021 IoT project, created by Kuoyuan Li kuoyuanl@student.unimelb.edu.au

Option 2 is selected (Data analysis and visualisation) due to limited remaining credits on Azure

## Datasets resources
In my project, 2 datasets which are all related to the medical insurance in USA are utilised. The datasets are found from Kaggle.

Note: I modify (add/remove) some parts of the data in Power BI for better visualization.

The sources are:

1. insurance.xlsx

Kaggle Link: https://www.kaggle.com/mirichoi0218/insurance

Original source: https://github.com/stedy/Machine-Learning-with-R-datasets

License: [Database: Open Database, Contents: Database Contents](https://opendatacommons.org/licenses/dbcl/1-0/)

2. state.xlsx

Kaggle link: https://www.kaggle.com/hhs/health-insurance

Original source: The health insurance coverage data was compiled from the US Department of Health and Human Services and US Census Bureau.

License: [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/)

## Reason behind the dataset choice, their related problems
Medical insurance is an important type of insurances for each individual. Understanding the price of insurance based on different factors is significant for both insurance providers and customers. Insurance providers can use the information to adjust their price and sale strategies in order to promote their business. Meanwhile, individual customers can use the information to estimate their insurance price based on their conditions, such that they can select an appropriate insurance plan. This topic is related to both business and healthcare, thus I decided to explore some datasets related to this topic.

After exploration, 2 datasets that are related to medical insurance details in the USA are used for analysis and visualization. The first dataset (insurance.xlsx) describes the individual medical spend on health insurance based on their details including gender, age, BMI, number of children covered by health insurance, whether is a smoker or not and the beneficiary's residential area in the US(in terms of northeast, southeast, southwest and northwest). The second dataset (state.xlsx) describes the health insurance coverage data for each state in the USA, including variables such as the uninsured rates before and after Obamacare, estimates of individuals covered by employer and marketplace healthcare plans, and enrollment in Medicare and Medicaid program. Two datasets are both related to medical insurance in the USA from different points of view: the first one focuses on the cost of insurance and the second one focuses on the coverage rate. From a business owner point of view, understanding both of them is important to make decisions such as target states, plan prices and so on. For a customer, knowing them can help them decide their next step on insurance choice.

## Key insights from the data
In both datasets, physical location shows up. Statistics vary based on their location. In the insurance dataset, the location is represented by 4 regions: northeast, southeast, northwest and northeast. In the state dataset, the location is represented by states. To connect these 2 relations, I add a new column named region for the state dataset and manually assign regions to each state based on the online resources (Wikipedia). It is very interesting and important to explore and understand the insurance rate and other factors which may influence insurance in different regions/states. Power BI provides a very useful visualization - the bubble map where bubble size indicates the value. We can compare bubble sizes to compare the same statistic in different states/regions. States within the same region have the same colour bubble for better visualization.

![image](https://user-images.githubusercontent.com/66192678/133436385-3d84f4af-18a9-4b63-aca7-0a987d4f0efb.png)

As can be seen in the above image, California has a lower uninsured rate, lower monthly tax credit, and higher employer and marketplace health insurance coverage comparing to other states. The decision maker can utilise this information to alter their strategies. Common patterns within 3 maps can also be identified. One interesting pattern that I observed is that state with lower uninsured rate usually has higher employer and marketplace health insurance coverage and lower monthly tax credit.

A funnel chart is used to compare the average expenses in different regions. As can be seen in the below image, the southeast US has the highest insurance expense, following by the northeast US, the northwest US and the southwest US which is 83.3% of the expense of the southeast US.

![image](https://user-images.githubusercontent.com/66192678/133437326-9ceca15c-5116-424d-8dd7-e48fbe0c0c7d.png)

A matrix is used to show the exact statistics. This does not contain extra information but is useful when we want to get the exact statistic. We can save time from looking back at the data file again.

![image](https://user-images.githubusercontent.com/66192678/133437553-4bbc6db8-064a-4668-800d-6c0b5f5f0562.png)






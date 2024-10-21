# WoW Food Delivery Services  

+ [Project Overview](#project-overview)  
* [Data Source](#data-source)  
- [Project Objectives](#project-objectives)  
- [Tools](#tools)  
- [Approach](#approach)  
- [Exploratory Data Analysis](#exploratory-data-analysis)  
- [Results](#results)  
- [Recommendations](#recommendations)  

### Project Overview
WoW Food Delivery Services is an online food delivery service that allows customers buy food from their favorites restaurants and have their food orders delivered to their desired location.  
Wow Foods generates revenue through commission on each customer's order value. 
However, there are various expenses WoW Foods incurs in delivery orders to customers. These expenses as delivery fee, payment processing fee and charges for refunds/ chargebacks. For incentives, WoW Foods also gives discounts to users; for using the app, new user and promo.  

### Project Objectives
This a comprehensive evaluation aimed at understanding and optimizing the financial dynamics of WoW Food Delivery Service. The goals are to:
- Identify areas where the service can reduce costs, increase revenue and implement pricing or commission strategies to enhance profitability.	
- Develop strategic recommendations aimed at enhancing profitability, based on the cost and profitability analysis

### Tools
Python: Pandas, Sweetviz, Seaborn, Matplotlib


## Approach
**Data collection**: Gathered comprehensive data related to all aspects of food delivery operations.
**Data cleaning and preparation**: 
- Cleaned the dataset for inconsistencies, missing values, or irrelevant information.
- Leveraged Python module called sweetviz for a quick exploratory data analysis.
- Converted “Order Date and Time” and “Delivery Date and Time” to a datetime format.
- Converted “Discounts and Offers” to a consistent numeric values
- Ascertained that all monetary values are in a suitable format (float or integer) for calculations
  
### Data Analysis
- Extracted relevant features that could impact cost and profitability.
- Performed a breakdown of costs associated with each order, including fixed costs (like packaging) and variable costs (like delivery fees and discounts).
- Determined the revenue generated from each order, focusing on commission fees and the order value before discounts.
- Computed the difference between ‘Order Date and Time” and “Delivery Date and Time” to diagnose the impact of delivery time on delivery cost.
- Computed the profit by subtracting the total costs from the revenue. 
-Analyzed the distribution of profitability across all orders to identify trends.
- Calculated the correlation between “Discounts” and “Profit”
- Forecast a new discount and a new commission based on profitable delivery service in the dataset provided.
- Modelled the financial impact of proposed changes, such as adjusting discount or commission rates

### Results
- The is a strong negative correlation of -0.78 between discount and profit. Increase in discount connotes reduction in profit and vice-versa.

- The minimum delivery time was 30 minutes while the maximum delivery time was 1 hour 59 minutes, while orders and deliveries are mostly completed in 44 minutes. However, it is necessary to note that there are no correlations between order/delivery time and profit/loss. 

- Most customers make use of WoW foods app, with a 10% discount. It is to be noted that refund and chargebacks are independent of payment methods.

- Delivery that ended up a loss made 76.32% of the total number of transactions.

- The breakdown of order delivery costs is as follows:
Refunds/Chargebacks – 10.84%  
Delivery fee – 10.97%  
Payment Processing Fee – 11. 43%  
Discounted Price 66.76%

![cost breakdown](https://github.com/user-attachments/assets/2dbe690d-70a6-4da3-a694-1f2b678f1101)

- On the other hand, the commission on the order value is 19.7% on average. Commission by percentage was as low as 2.6% and the maximum which occurred once was 169%

### Recommendations
- According to the results of the cost breakdown, discounts amounted to 66.76%, thereby warranting a review.

- According to the moddelled discount and commission percentages, the discount given on any of the products must not be above 10% and the commission must be increased to 30% for profitability.

![Profit analysis](https://github.com/user-attachments/assets/a1b656ba-80bd-47e0-b76a-17827f0e8c10)

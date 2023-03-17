## Food_Aggregator_App_Customer_Order
Data Analysis and visualization using Python on customer data for different orders placed by registered customers in an online portal for a food aggregator company

## Context
The number of restaurants in New York is increasing day by day. Lots of students and busy professionals rely on these restaurants due to their hectic lifestyles to order food online. A food aggregator company FoodHub offers access to multiple restaurants through a single smartphone app.

The app allows the restaurants to receive a direct online order from a customer. The app assigns a delivery person from the company to pick up the order after it is confirmed by the restaurant. The delivery person then uses the map to reach the restaurant and waits for the food package. Once the food package is handed over to the delivery person, he/she confirms the pick-up in the app and travels to the customer's location to deliver the food. The delivery person confirms the drop-off in the app after delivering the food package to the customer. The customer can rate the order in the app. The food aggregator earns money by collecting a fixed margin of the delivery order from the restaurants.

## Objective
The food aggregator company has stored the data of the different orders made by the registered customers in their online portal. Data analysis and visualization is performed on the customer data to find answers to explore the demands of different restaurants and answer some key questions that will help the company to improve the business.

## Data Description
The data contains the different data related to a food order. The detailed data dictionary is given below.

## Data Dictionary
- order_id: Unique ID of the order
- customer_id: ID of the customer who ordered the food
- restaurant_name: Name of the restaurant
- cuisine_type: Cuisine ordered by the customer
- cost: Cost of the order
- day_of_the_week: Indicates whether the order is placed on a weekday or weekend (The weekday is from Monday to Friday and the weekend is Saturday and Sunday)
- rating: Rating given by the customer out of 5
- food_preparation_time: Time (in minutes) taken by the restaurant to prepare the food. This is calculated by taking the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation.
- delivery_time: Time (in minutes) taken by the delivery person to deliver the food package. This is calculated by taking the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information

## Key Observations
#### Customer orders vs Cuisine types
![image](https://user-images.githubusercontent.com/50159148/225828336-17bb83b7-d455-4094-a0de-9acc080e8f6f.png)
- This highlights how American cuisine is the most popular amongst other cuisines


#### Customer orders vs Weekday/Weekend
![image](https://user-images.githubusercontent.com/50159148/225830167-67211346-2381-4703-843b-511a7a2671f0.png)
- This shows how weekends are nearly 3 times more popular to order compared to weekdays


#### Customer orders vs Rating
![image](https://user-images.githubusercontent.com/50159148/225830705-687c240d-7613-44ff-bb57-c42734666870.png)
- This shows nearly half of all customers do not leave a rating on the app


## Business Recommendations

[1] Customers tend to order significantly more during weekends compared to weekdays. While Foodhub is already serving customers well by providing faster delivery on weekends, it may be helped by likely lesser traffic on weekends. Because of increasing demand on weekends, customer experience may be improved by increasing fleet size on weekends to serve more customers as well as provide even faster delivery times

[2] Given the lack of correlation between customer ratings and total delivery times, a slightly slower delivery time may not affect customer ratings. Lower fleet sizes on weekdays may make more sense given the lower demand on weekdays which can help lower company costs.

[3] Alternatively, the company can also try to increase demand on weekdays by providing more customer discounts that might boost orders

[4] Customer ratings are crucial to gauge customer feedback on Foodhub's service. One area where Foodhub could improve is to incentivize customers to provide more ratings. More customer feedback data through ratings can help better understand customer behavior and preferences such as cuisine types, favorite restaurants, favorite time to ordewr etc.

[5] Small discount vouchers on next orders could be offered to customers if they leave ratings which will not only get Foodhub more data about customer opinion but also increase Foodhub's revenue.

[6] Current revenue model is 15% on orders greater than 5 dollars and 25% on orders greater than 20 dollars. EDA suggests that only 30% of orders are greater than 20 dollars. Median cost of order is around 14 dollars. This suggests most common orders (14-16 dollars) generate the same percent revenue as much cheaper orders (<$10). Foodhub could increase their revenue by proposing a more tiered model to restaurants e.g. 15% on order between 5-10 dollars, 20% on orders between 10-20 dollars and 25% on orders> 20 dollars.

[7] Because there is significantly higher demand on weekends, it might also be useful to have a have a 5-10% increase in charges to restaurants during weekends. This will significantly boost revenue

[8] The company could also promote restaurants serving more popular cuisines that have high customer ratings (e.g. >4-4.5) but have recieved fewer number of orders. Better outreach may help them reach more customers. Customers could also be incenticized to order from such restaurants at discounted rates.

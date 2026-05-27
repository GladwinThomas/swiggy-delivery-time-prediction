Business Use Case:
In the competetive food delivery market, on-time delivery is critical for customer satisfaction, retention, and operational efficiency. A company wants to optimize delivery time predictions to improve customer experience by providing accurate estimated delivery times and to manage resources effectively. Accurate predictions of delivery time can also allow the business to:

1. Improve delivery efficiency:
- Identifying the factors that slow down deliveries can enable better resource allocation., such as reliable scheduling for delivery personnel.
2. Enhance Customer Satisfaction:
- Reliable delivery ETAs can improve the customer experience by reducing wait-time uncertainity. 
- Clear transparency helps customers informed and reduces the chances of cancelled orders.
3. Optimize Operational Costs:
- If the model can predict scenarios with higher delays, additional resources (like more drivers or prioritizing specific orders) can be allocated. 
- Accurate predictions reduces customers service calls regarding delivery delay. 
- Also company can implement surge pricing in extreme weather or congestion events. 
- Restaurants can manage staff to balance out between in house orders or home delivery. 
- Off peak hours can be leveraged to increase customer traffic by using coupons or discounts.
Problem Statement:
Predicting the delivery time for food from origin to destination.
Target:
Delivery Time in minutes.
Type of algorithms used:
Regression
Type of Learning:
Supervised Learning
Dataset Name:
swiggy.csv
Dataset Shape:
45594 X 20
Dataset Features:
1. 'ID': order id
2. 'Delivery_person_ID': ID of the delivery person
3. 'Delivery_person_Age': Age of the delivery person
4. 'Delivery_person_Ratings': Average rating of the delivery person
5. 'Restaurant_latitude': Latitude of the restaurant
6. 'Restaurant_longitude': Longitude of the restaurant 
7. 'Delivery_location_latitude': Latitude of the destination 
8. 'Delivery_location_longitude': Longitude of the destination
9. 'Order_Date': Date of order 
10. 'Time_Orderd': Order time
11. 'Time_Order_picked': Time at which food is picked
12. 'Weatherconditions': Weather condition during the delivery
13. 'Road_traffic_density': Road traffic density
14. 'Vehicle_condition': Condition of the vehicle 
15. 'Type_of_order': Order type like lunch or snack and so on.
16. 'Type_of_vehicle': Delivery Vehicle Type
17. 'multiple_deliveries': Whether multiple deliveries are to be delivered 
18. 'Festival': Is it a day of festival 
19. 'City': Type of City
20. 'Time_taken(min)': Time taken to deliver (in min) [TARGET]
Evaluation Metrics
The most suitable evaluation metric that can be used for our case is MAE (Mean Absolute Error).

This is because due to some factores like weathers, traffic and festivity, delivery time might increase, which results them to act like a outlier , even though they are not.

Also we can maintain the unit of time which is easier to relate.

So, to be more robust to the outliers and to consider outlier like values, MAE is used.

# Hotel Booking Cancellation Prediction
In the hospitality industry, managing hotel bookings efficiently is crucial for maximizing revenue and providing top-notch customer service. One of the challenges hotels face is predicting whether a booking is likely to be canceled or not. Understanding the factors that contribute to booking cancellations can help hotels make informed decisions and allocate resources effectively.

In this project, we aim to explore the factors that contribute to booking cancellations in the hospitality industry. Our [Hotel booking](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand) dataset contains information on bookings for both a Resort Hotel and a City Hotel, including various features such as lead time, arrival date, number of guests, room types, deposit types, and more.

The main objectives are as follows:
### EDA
1. What is the distribution of hotel types (Resort Hotel or City Hotel) in the dataset?
2. How does the lead time (number of days between booking and arrival) vary across hotel types?
3. Which month has the highest number of bookings?
4. What is the average daily rate (ADR) for different room types?
5. Is there a relationship between the number of previous cancellations and the likelihood of cancellation?

### ML
- <b>Predicting Booking Cancellations</b>: build a machine learning model that can predict whether a person will cancel their booking based on the available features in the dataset. This model can be valuable for hotels to anticipate cancellations and plan resources effectively. It can also help in offering more rooms than available to maximize revenue, as mentioned in the project description.


# Conclusion
We explored factors influencing booking cancellations and developed a predictive model to determine if a booking is likely to be canceled. Our analysis provided valuable insights:
- The majority of bookings (61.15%) were from city hotels, with a higher cancellations rate to resort hotels (30% vs 23%).
- Bookings with long lead times (80 days or more) were more likely to be canceled, while shorter lead times (38 days or less) correlated with lower cancellation rates.
- Summer months (July and August) saw the highest number of bookings, while winter months (December and January) had the lowest.
- Certain room types, both in city and resort hotels, had higher average daily rates (ADR).
- Guests with multiple previous cancellations were more likely to cancel their current booking.

Our XGBoost Classifier performed well in predicting cancellations, with `required_car_parking_spaces`, `total_of_special_requests`, `lead_time`, `agent`, `market_segment_Online TA`, `adr` being key predictors. Using Explainable AI (XAI) techniques, we gained transparency into the model's decisions.

By leveraging these insights, hotels can better plan resources, enhance customer satisfaction, and optimize operations. The combination of EDA, ML, and XAI empowers the hospitality industry to make data-driven decisions, ultimately improving overall efficiency and guest experience.
# Investigate-Business-Hotel-using-Data-Visualization

## Data Preprocessing
- Handle Missing Values
  There are several features whose values are empty, namely the company, agent, city, and children features. Some steps to handle the missing value of the feature, namely:
  - Company: will be filled with 0 because it is assumed that the customer orders the hotel personally without going through a company.
  - Agent: the same as the company feature, it will be filled with 0 because it is assumed that the customer orders the hotel personally without going through an agent.
  - City: will be filled with the most frequent city in the city feature, namely the city of Denpasar because each customer should have a city of origin so that an empty city feature is assumed to come from the city of Denpasar.
  - Children: will be filled with 0 because it is assumed that the customer does not bring children.
- Replace The Inappropriate Value
  - There are several values that do not match the 'meal' feature which will be changed to 'No Meal'
    because it is assumed that the feature that is not clearly defined 'Undefined' is a customer who does not order any food either at Breakfast, Dinner or Full Board (Breakfast + Dinner).
  - There are several data types that are not suitable, namely in the Children, Agent, and Company features
    which should have an integer data type instead of a float data type, so the data type must be changed.
- Drop Unnecessary Data
  - Drop data that has 0 total_guests and 0 stay_duration.

## Monthly Hotel Booking Analysis Based on Hotel Type

  ![image](https://github.com/nunuufdlh01/Investigate-Business-Hotel-using-Data-Visualization/assets/89932073/82b65c58-bc06-4c03-b12b-e279ecb708de)

- Interpretation:
  - Hotel bookings on average increase during the peak season and high season holidays. The peak holiday season occurs in June - July because there are school holidays and Idul Fitri holidays with a long duration. The high season holiday season has a shorter duration compared to the peak season holiday season which occurs in November - December because this month there are also school holidays and Christmas holidays which are not as long as in June - July.
  - Hotel bookings begin to decrease during the low season holiday season which occurs throughout January - June and also occurs in July - November. In this low season, the hotel should provide discounts/discount vouchers so that customers are still interested in visiting the hotel.

## Impact Analysis of Stay Duration on Hotel Bookings Cancellation Rates

  ![image](https://github.com/nunuufdlh01/Investigate-Business-Hotel-using-Data-Visualization/assets/89932073/64e20b11-5b78-4063-bf7e-5fa960d2cc63)

- Interpretation:
  - The longer the duration of the stay, the higher the order cancellation rate at the hotel.
  - The highest order cancellation at City Hotel occurred in group 4 (more than 21 days) of 87.23%.
  - The highest order cancellation at Resort Hotels occurred in group 3 (15 to 21 days) of 46.75%.
  - City Hotels have a higher order cancellation rate compared to Resort Hotels.
 
## Impact Analysis of Lead Time on Hotel Bookings Cancellation Rate

  ![image](https://github.com/nunuufdlh01/Investigate-Business-Hotel-using-Data-Visualization/assets/89932073/7a7977b2-59e4-430a-a174-44bc208f0d64)

- Interpretation:
  - The longer the time interval for bookings in a year, the ratio of hotel booking cancellations also increases (if the time is divided into quarters). This may be due to the longer the time interval for the order, the more likely it is for the customer to have a busy agenda that year, thus allowing hotel bookings to be cancelled.
  - This is unique if the time between bookings is more than a year, the cancellation rate suddenly drops dramatically. This may be because the hotel provides additional discounts or special treatment if the order interval is more than a year or other things that need to be explored further about this.
  - The highest cancellation ratio occurred in the fourth quarter before a year, namely City Hotels at 76.27% and Resort Hotels at 42.53%.

**mini-project file link is** <a href="https://drive.google.com/file/d/1UTaVLAHYNBevDLV-OFX3oEAbk_hQL3Cw/view?usp=sharing">Here</a>




# Tenant Churn Behavior

In the current era, there is an increasing number of digital platforms offering properties (apartments or boarding houses) for rent, making tenants seeking accommodation valuable assets for this industry. This scenario applies to industries that offer reservations or submit bookings through digital platforms (web or applications).

The analysis of Company M's tenants involves those who have already submitted bookings on company's platform but are no longer subscribed to company's services. Therefore, company needs to anticipate an increase in the number of tenants who no longer subscribe.

## Business Understanding
In the digital property industry, especially apartments or boarding houses offered for rent through digital platforms, tenants seeking accommodation are valuable assets as customers who make reservations or submit bookings, allowing companies to generate profits. This scenario raises several business questions using data:
1. What is the composition of tenants who continue to use and leave Company M services?
2. How does the number of tenants progress towards the churn rate from year to year?
3. How does the tenant booking submission rate affect the churn rate?
4. What is the distribution of cities based on tenant churn over the last five years?
5. How is the distribution of tenant account age relative to the churn rate?
6. How does the tenant signup method rate affect the churn rate?
7. How does the tenant type signup rate affect the churn rate?

## Data Understanding
* Journey Tenant Booking data contains information from June 28, 2018 to June 30, 2023, but some dates in the data are unknown
* Journey Tenant Booking data comes from company M
* This data has 15 columns and 217,155 rows
* Data Dictionary:
   * tenant_id: ID to identify the tenant
   * date_account_created: The date when the account was created or registered
   * gender: Information about the tenant's gender
   * signup_method: The method used when registering or creating an account
   * signup_type: Type of registration carried out by the tenant (via application or platform)
   * first_device_type: Device type used when registering or creating an account
   * submit_booking: The possibility that a tenant will make a booking or not
   * domicile_code: Tenant's domicile city code
   * total_favorites: Number of properties (boarding houses) liked by tenants
   * total_chat: Total tenant interactions with the owner via the ask owner feature
   * total_submit_booking: Total number of booking submissions by tenants
   * total_visit: Total tenant visits to the Company M homepage
   * total_visit_listing: Total visits to detailed pages
   * total_click_booking: Total intensity of tenants making bookings before the day
   * churn: The possibility of a tenant canceling or choosing not to continue payments

## Exploratory Data Analysis
### 1. Tenant Churn Composition
   ![image](https://github.com/renatasa13/Tenant-Churn-Behavior/assets/93513745/9ed44548-ae11-49b2-bffd-b906b72db498)

The graphic shows the composition of churn data indicating that exactly 50% of users are still using Company M services. There is a balanced percentage between users who are still using Company M services and those who are not. The data highlights a crucial point where half of user interactions still involve Company M services.

### 2. User Registration and Churn Trend
![image](https://github.com/renatasa13/Tenant-Churn-Behavior/assets/93513745/db74fafe-6de9-4605-bd4b-6a5ef859ff00)

Based on the available data, there is a discernible pattern in the user registration trends over the past few years. From 2018 to 2021, there is a consistent increase, indicating progression in user registrations. However, in 2022, there was a significant 20% decrease in user registrations. This decline suggests a notable shift in user engagement during that period. Interestingly, user registrations showed improvement in 2023, with a 1% increase.

Similarly, trends in churn (user discontinuation) and retention provide intriguing insights into user behavior. Although specific details of these trends are not explicitly provided, we can infer that the patterns of users leaving the service (churn) and those choosing to continue using the service (retention) have experienced fluctuations over the past few years.

### 3. Submit Booking by Churn
![image](https://github.com/renatasa13/Tenant-Churn-Behavior/assets/93513745/80868514-e4cd-495c-9f2d-93e91c194283)

Based on the chart provided, it can be observed that a significant portion of the data does not indicate whether tenants have submitted bookings or not. However, 49.99% of this data suggests that tenants are no longer using the service. In contrast, among the data showing that tenants have submitted bookings, 50.05% are still using the service, while 49.95% have discontinued the service. Furthermore, among tenants who did not submit bookings, 50% have ceased using the service. This suggests that the behavior of tenants, whether they submit bookings or not, is influenced by their needs for Company M services.

### 4. Domicile Tenant by Churn
![image](https://github.com/renatasa13/Tenant-Churn-Behavior/assets/93513745/0b502d1a-d585-470d-8015-94dc1f4d2f92)

Based on the chart, there doesn't seem to be a significant difference between cities in terms of the percentage of tenants who have stopped using the service, with approximately 49%-50% in each city. This indicates that there is no clear trend among tenants in deciding to cancel payments based on their location or the city they reside in.

### 5. User Account Age Category by Churn
![image](https://github.com/renatasa13/Tenant-Churn-Behavior/assets/93513745/291191f4-3b41-42b2-842e-7d9d7484599e)

The data analysis indicates a stable churn rate across various account age categories. New Users have a churn rate of 50.12% and a non-churn rate of 49.88%. Intermediate Users have a churn rate of 49.79% and a non-churn rate of 50.21%. Meanwhile, Long-term Users experience a churn rate of 50.19%, with a non-churn rate of 49.81%. This comparison illustrates relatively small differences between churn and non-churn rates in each category.

The primary recommendation for retention strategy is to focus on introducing the product's value to New Users through personalized and intensive communication. Additionally, it is crucial to support Intermediate Users by enhancing their understanding and addressing factors influencing the churn rate, as this may be key to reducing the overall churn rate.

### 6. Signup Method by Churn
![image](https://github.com/renatasa13/Tenant-Churn-Behavior/assets/93513745/675958e3-b393-4d4e-aae1-0bb63e69a34d)


Based on the chart, the majority of Company M tenants use the basic registration method (using email and password). From the basic registration method, it is known that 50.05% of users are still using the service. For those who registered using the Google method, 50.2% are no longer using the service. Registration via phone number is the least utilized method. For the registration method that is unknown, 49% of tenants did not continue the service. The number of tenants leaving the service and those who are not is not significantly different.

### 7. Signup Type by Churn
![image](https://github.com/renatasa13/Tenant-Churn-Behavior/assets/93513745/5e6bb8d6-f058-4c07-b7e3-978f7962c6f9)

Based on the sign-up type chart, there are categories such as unknown, web, iOS, and Android. The majority of tenants with an unknown sign-up type use an unspecified method. Tenants who register through the web platform have a higher percentage of leaving the Company M service, around 50.01%. Users on the iOS platform show a percentage of those still leaving the service at 50.35%. Meanwhile, Android users have a percentage of those who have already left the service at 53.49%. From this information, it can be concluded that most tenants prefer signing up through the website.

# Dashboard
![image](https://github.com/renatasa13/Tenant-Churn-Behavior/assets/93513745/89bd2cf7-60ed-4d40-8359-6ed025e3fb12)

Link Dashboard [https://lookerstudio.google.com/s/qyneghkSekU ](https://lookerstudio.google.com/s/rxGhW_1Im3s)

# Recommendation
* Conducting an evaluation of the products and services by surveying users and conducting market research through collected feedback is a commendable approach. The findings can be reviewed to enhance ease of use and user comfort, thereby increasing user retention. Subsequently, marketing campaigns can be implemented to enhance service visibility. The fluctuation in the growth of tenants each year necessitates Company M to design strategies to improve and maintain customer retention based on evolving trends. Offers can be targeted, such as providing promotions during the start of the academic year for students, to increase the number of tenants. It's essential to consistently provide excellent service and maintain relationships with tenants to sustain their retention.
* Analyzing the preferences, needs, and behaviors of Intermediate users can help identify effective solutions to retain them within the service ecosystem. Additionally, providing specific loyalty programs for Intermediate users with benefits that enhance satisfaction and retention is recommended.
* Boosting promotions for the New User Booking program on the basic registration screen of the website is advised. Offering more attractive and exclusive deals for users selecting this registration method, such as special discounts, additional reward points, or other exclusive benefits, can encourage users to choose the basic registration option on the website due to its simplicity and advantages.
* Conducting an in-depth analysis of the data transfer, especially during the data collection and transfer phases, is crucial. Identifying the processes involved in data transfer and checking for disruptions or failures in these processes causing features in the data to contain null values is important.


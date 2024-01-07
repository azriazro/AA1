# AA1
Submission of AA1

I created an artificial dataset using Python with features extracted from datasets obtained from kaggle.

The Objectives of this project is to predict the churn of customers based on their profile using three predictive models.
-HP Forest (High-Performance Forest)
-Gradient Boosting
-Decision Tree

The dataset in this project is an artificial dataset generated in Python. You can find the generated dataset in this repository.

Below is the code that i used to generate the dataset mentioned above.

import pandas as pd
import numpy as np


np.random.seed(42)


customer_ids = range(50001, 55001)


churn = np.random.choice([0, 1], size=5000, p=[0.8292, 0.1708])


tenure = np.random.randint(0, 60, size=5000)
preferred_login_device = np.random.choice(['Mobile Phone', 'Phone', 'Computer'], size=5000)
city_tier = np.random.choice([1, 2, 3], size=5000)
warehouse_to_home = np.random.randint(5, 27, size=5000)
preferred_payment_mode = np.random.choice(['Debit Card', 'UPI', 'CC', 'E wallet', 'COD', 'Credit Card','Cash On Delivery'], size=5000)
gender = np.random.choice(['Male', 'Female'], size=5000)
hour_spend_on_app = np.random.choice([1, 2, 3, 4, 5, 6], size=5000)
num_of_device_registered = np.random.choice([1,2,3, 4, 5, 6], size=5000)
preferred_order_cat = np.random.choice(['Laptop & Accessory', 'Mobile', 'Fashion', 'Others','Grocery','Mobile Phone'], size=5000)
satisfaction_score = np.random.choice([1, 2, 3, 4, 5], size=5000)
marital_status = np.random.choice(['Single', 'Divorced', 'Married'], size=5000)
num_of_address = np.random.randint(1, 22, size=5000)
complain = np.random.choice([0, 1], size=5000)
order_amount_hike = np.random.randint(11, 26, size=5000)
coupon_used = np.random.randint(0, 16, size=5000)
order_count = np.random.randint(1, 16, size=5000)
days_since_last_order = np.random.randint(0, 46, size=5000)
cashback_amount = np.random.randint(0, 325, size=5000)


data = pd.DataFrame({
    'CustomerID': customer_ids,
    'Churn': churn,
    'Tenure': tenure,
    'PreferredLoginDevice': preferred_login_device,
    'CityTier': city_tier,
    'WarehouseToHome': warehouse_to_home,
    'PreferredPaymentMode': preferred_payment_mode,
    'Gender': gender,
    'HourSpendOnApp': hour_spend_on_app,
    'NumberOfDeviceRegistered': num_of_device_registered,
    'PreferredOrderCat': preferred_order_cat,
    'SatisfactionScore': satisfaction_score,
    'MaritalStatus': marital_status,
    'NumberOfAddress': num_of_address,
    'Complain': complain,
    'OrderAmountHikeFromlastYear': order_amount_hike,
    'CouponUsed': coupon_used,
    'OrderCount': order_count,
    'DaySinceLastOrder': days_since_last_order,
    'CashbackAmount': cashback_amount
})

# Displaying the DataFrame
print(data)
-------------------------------------------------------------------------------------------------------------------------------

For SAS workflows, the snippets of the SAS are in the document.

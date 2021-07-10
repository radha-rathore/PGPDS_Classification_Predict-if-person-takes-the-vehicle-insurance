# Classification - Whether a person will take the vehicle insurance or not
# An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee.

# For example, you may pay a premium of Rs. 5000 each year for a health insurance cover of Rs. 200,000/- so that if, God forbid, you fall ill and need to be hospitalized in that year, the insurance provider company will bear the cost of hospitalization etc. for up to Rs. 200,000. Now if you are wondering how can company bear such high hospitalization cost when it charges a premium of only Rs. 5000/-, that is where the concept of probabilities comes in picture. For example, like you, there may be 100 customers who would be paying a premium of Rs. 5000 every year, but only a few of them (say 2-3) would get hospitalized that year and not everyone. This way everyone shares the risk of everyone else.

# Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

Objective:
Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimize its business model and revenue.

We have information about:

FEATURES:

Gender- Male/Female
Age - Age of the vehicle owner
Driving_License - 1: Has DL, 0: No DL
Region_Code
Previously_Insured - 0/1
Vehicle_Age - 1 to 2 Year, <1 year, >2 years
Vehicle_Damage - Yes/ No
Annual_Premium
Policy_Sales_Channel
Vintage - This metric represents the number of days a customer has been insured up until now and is therefore ordinal in nature.
id - Id of the user
TARGET :

Response - 0/1

# The dataset is highly imbalanced, so I have done resampling of data before prediction.
# Recall is the metric of focus here because I want to correctly and accurately identify those people who will actually take the insurance. I want to increase predicted true values (True positive) maximum when compared to actual true values (True positive+ False negative).

# I want to reduce false negatives in order to avoid losing potential customers

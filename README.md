# Starbucks Capstone Project

Dataset contains simulated data that mimics customer behavior on Starbucks rewards mobile app. Starbucks sends out to offers to mobile app users. Offer can be advertisement of the drink or an actual offer as discount or BOGO(buy one get one). Not all users receive same offer and some users might not receive any offer in the week. Along these lines, Starbucks can most likely built the possibility that customer opens the offer after they get it and finish the transaction.

##### Problem Statement
The goal of this project is to combine transaction, demographic and offer data to determine which demographic groups respond to which offer type. This goal can be achieved by following mentioned strategy:
1. Exploring & visualizing data
2. Data pre-processing
3. Analysis on cleaned data
4. Scaling numerical features
5. Trying supervised learning models
6. Evaluate model performance and chose the best one
7. Use GriSearchCV to find optimal parameters for model training

##### Dataset Description
The data is contained in three files:
portfolio.json — containing offer ids and meta data about each offer (duration, type, etc.)
profile.json — demographic data for each customer
transcript.json — records for transactions, offers received, offers viewed, and offers completed
Here is the schema and explanation of each variable in the files:
portfolio.json
id (string) — offer id
offer_type (string) — type of offer ie BOGO, discount, informational
difficulty (int) — minimum required spend to complete an offer
reward (int) — reward given for completing an offer
duration (int) — time for offer to be open, in days
channels (list of strings)
profile.json
age (int) — age of the customer
became_member_on (int) — date when customer created an app account
gender (str) — gender of the customer (note some entries contain ‘O’ for other rather than M or F)
id (str) — customer id
income (float) — customer’s income
transcript.json
event (str) — record description (ie transaction, offer received, offer viewed, etc.)
person (str) — customer id
time (int) — time in hours since start of test. The data begins at time t=0
value — (dict of strings) — either an offer id or transaction amount depending on the record
## Contents of Repository
- [Jupyter Notebook](https://jupyter.org/) - Editor for Python Code
- Datasets put in folder [Airbnb Datasets](https://github.com/chetnashahi/Starbucks-Project/tree/master/Data)
- And of course, the course [Udacity](https://classroom.udacity.com/)

The detailed blog post is also published on [Medium](https://chetna-shahi31.medium.com/starbucks-offer-analysis-468c516135e4)
## Future Scope of Work
I can try doing more model performance tuning and see if any new features can improve the performance. We can also do some unsupervised learning on clustering the customers.


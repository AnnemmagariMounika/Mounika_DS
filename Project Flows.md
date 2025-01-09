# Churn Prediction

## This project is a classification model.

the project which I worked on, it was actually for a client
called Walgreens,
So my client was facing actually saturation in the last three months.
There is a lot of customers who
is churning from the store. He wanted to understand who are the
customers who are going to churn in the
next quarter, today itself,
so that he can actually take activities or actions based on
those people who is going to churn.

For this project, we started collecting data.
For this, we connected to Python Oracle databases by using Python.
The package that is used is cx_oracle. So we use Python, cx_oracle,
we connect to the database. From there, we pulled all
the required columns to the Python environment. Once we have done
everything to the Python environment, then we started actually
doing memory optimization, null value treatment, outlier treatment,
min-max scaling, standard scaling, dummy variables,
label encoders, these things. This will help us to establish the
data ready for our data science or analytical work.

We have automated this pre-processing pipeline. The automation helps
us in repeating the same steps in across multiple projects also.
Post-building the entire pre-processing pipeline, then we started
with model building.
In model building, first We check for linearity and non-linearity.
Because data was actually nonlinear in
nature, we went for decision tree, random forest , boosting
style of algorithms.
Based on that linear and nonlinear relations, we draw the
relationship between scatterplots, y, x1, y, x2, y, x3.
So once we have this nonlinear relations, we start
building decision tree, random forest, Xgboost.
Post-model building, my baseline model is decision tree.
It was giving 71% accuracy.
From there, we moved to random forest. It was actually giving
around 80 to 85% accuracy. From there, we went to boosting, which is
around 87% accuracy.
I was using precision, recall, F1 score
as a measure to validate the model. Accuracy score was also there.
Data was imbalanced in nature.
We have taken the SMoTE analysis to balance this particular data site.
Post-model building, we have done K-fold validation also.
On an average, accuracy was coming around 86% across all the K-folds
that which is given.
This was saved as a pickle file. The pickle file was actually given to the
clients for inference purposes.
We deployed this again using Flask.
I was involved in building a little bit of UI using Streamlit also. 

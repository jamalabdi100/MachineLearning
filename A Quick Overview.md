# A Quick Overview
## Results of two Classification Models

In this project we used two different classification model along with GridSearchCV to tune its parameters. We followed following steps:
- Feature Slection using important feature selection method
- Applied Minmax scaler to scale the data
- Trained the models and calculated their scores
- Trained models with GridSearchCV to tune their parameters
## Feature Selection

As we have some negitive value in the data, so in order to include their imporatance I used feature importance selection method to select top 10 features based on their results.
- Drag and drop images (requires your Dropbox account be linked)
- Import and save files from GitHub, Dropbox, Google Drive and One Drive
- Drag and drop markdown and HTML files into Dillinger
- Export documents as Markdown, HTML and PDF

## Model Traing
We trained two models 'DecisionTreeClassifier' and 'RandomForestClassifier'.
Following are their scores:
##### DecisionTreeClassifier
Training Data Score: 1.0
Testing Data Score: 0.834055459272097
##### RandomForestClassifier
Training Data Score: 0.8667520819987188
Testing Data Score: 0.8639514731369151
## Model Traing with GridSearchCV

Results for the grid searcv are as follows:
##### DecisionTreeClassifier
{'max_leaf_nodes': 23, 'min_samples_split': 2}
0.8808456117873158
##### RandomForestClassifier
{'max_depth': 8, 'max_features': 1.0, 'n_estimators': 30}
0.8827623165403315
## Summary
We can see that after applying gridsearchcv to tune the parameter the results of the models improved a lot. Same observation we see that, in first case accuracy of decsion tree classifier is higer then random forest, but in the tuned parameter case both are almost same. This is due to the fact random forest is more complex model and take more steps to fine tune the model on the random parameter. But in the second case when we already provide them the tuned parameter, they learned the data quite equally.
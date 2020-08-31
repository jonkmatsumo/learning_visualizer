# Comparing Learning Algorithms #

#### To view the live demo deployed on Heroku, click [here](https://learning-visualizer.herokuapp.com/). ####

Interactive web application that compares the effectiveness of three different common machine learning algorithms - Support Vector Machines (SVMs), Logistic Regression, and Random Forests, a type of Decision Tree - with respect to a simple supervised learning task: identifying if the mushrooms in the [Mushroom Data Set](https://archive.ics.uci.edu/ml/datasets/Mushroom), courtesy of the University of California, Irvine Machine Learning Repository. The user can adjust the hyperparameters for each respective algorithm using the sidebar at the left of the display and view how their selected algorithm performs with respect to basic statistical measures (accuracy, precision, and recall) in addition to more graphical breakdowns in the form of a Confusion Matrix (useful for showing false positives, false negatives, etc.), a ROC Curve, and the Precision-Recall Curve.

![Sample Map 1](/assets/sample_display.PNG)

In the sidebar on the left, the user is prompted to select the type of classifier used. The parameters shown below will vary for the specific algorithm chosen:

1. **Support Vector Machine** - Kernel ([radial basis function](https://en.wikipedia.org/wiki/Radial_basis_function_kernel) or linear) and the gamma or kernel coefficient.
2. **Logistic Regression** - Regularization Parameter which controls the amount of Regularization applied and the number of iterations to perform (higher will generally be more accurate, but with diminishing returns).
3. **Random Forrest** - Number of trees in the forest, maximum depth of the tree, and whether to bootstrap samples or not.

In the menu below that, the user will be given the option to choose to have any of the following displayed in addition to the basic statistical information:
1. **Confusion Matrix** - shows the number of false and true positives and negatives.
2. **ROC Curve** - shows the ability of a binary classifier as the discrimination changes.
3. **Precision-Recall Curve** - shows the tradeoff between precision and recall.

To run this application, either check out the [live demo](https://nyc-visualizer.herokuapp.com/) deployed on Heroku or download the repository and run the following in the Terminal:
> streamlit run app.py.

Note that this application makes use of the following libraries: Matplotlib, Numpy, Pandas, SciKit-Learn, and Streamlit. For more information, check *requirements.txt*. 

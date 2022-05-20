There are two different feature combinations used,
one optimal for Naive Bayes: name and steps
X_train = scipy.sparse.hstack([X_train_name, X_train_steps])
X_test = scipy.sparse.hstack([X_test_name, X_test_steps])

The other is for Decision Tree: name, steps, ingredients, n_ingredients
X_train = scipy.sparse.hstack([X_train_name, X_train_steps, X_train_ing, X_ning_train.values[:, None]])
X_test = scipy.sparse.hstack([X_test_name, X_test_steps, X_test_ing, X_ning_test.values[:, None]])

These are codes in order to reproduce the classification report and the confusion matrices in the report.
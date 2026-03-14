# Naive-Bayes

### Naive Bayes is based on Bayes Theorem .

[Scikit learn docs](http://scikit-learn.org/stable/modules/naive_bayes.html)

## It basically first considers the point in between the two Classifiers and then tries to predict the probability to guess in which class it belongs to . Then it tries to calculate the <b>Posterior Probability</b> from the product of <b>likelihood</b> and the <b>prior probability</b> . We can ignore the <b>Marginal likelihood{ p(x) }</b> because when we compare the posterior probability ofthe different classifications then it cancels out .

![down](https://chrisalbon.com/images/machine_learning_flashcards/Gaussian_Naive_Bayes_Classifier_print.png)

This is suitable for Sentiment Analysis problems with two output labels .

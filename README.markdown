Assingment:

For homework, answer the following questions:

What data set did you use:

I picked the abalone data set (
avaiable at http://archive.ics.uci.edu/ml/datasets/Abalone) and try
out both a KNN and a Bayes classifier. Compare and contrast them and
be able to answer the following questions:

What variables were included in my model:

In this case, I actually found that all of them were surprinsly
predictive over the actual value I wanted, which was the number of
rings (age). All of them except for Gender. I removed gender as it
provided no actual value.

Did one method do better than the other:

In this case, since the data is "pseudo categorical" age is continuous
but in this case it's represented as the category of the number of
rings, I think KNN did a better job at fitting throughout the whole
spectrum. If I had wanted to try to regularize the model, it's possible
that I could have gotten better value of the Naive Bayes, but as it was,
I got "ok" values. What follows is a heatmap of the confusion matrix.

KNN:

![knn](https://raw.github.com/earino/data_science_hw2/master/images/knn.png)

BAYES:

![bayes](https://raw.github.com/earino/data_science_hw2/master/images/bayes.png)

Conclusion: You'll note that the KNN fits better throughout the entire
multidimensional space (it is a better fit at the edges of the
prediction, particularly the top right.) Whereas it seems that the bayes
over-generalizes too quickly.

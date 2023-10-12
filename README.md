# Spam-Filter
This project has 3 parts - at the frontend a webpage to help take input from the user, at the backend an ML model to filter spam messages, an intermediate flask framework that connects these two.

The webpage created was based on HTML and CSS.  A message is accepted as input using HTML and is passed on to the main module which detects if the message is a spam or not. The website is beautified using CSS.

At the backend, an ML model is created using the Naïve Bayes algorithm. Python packages: scikit learn, pandas, NumPy and seaborn were useful in building the model. The model is trained with a dataset from the Kaggle website. The model is tested for an accuracy of 86% (mean squared error formula). Next the pickling process was done, where the python object model was converted to a class file. This class file i now used to filter the input messages.

Flask framework is utilized to make the connection between the HTML webpage and the python class file. Using flask, the input that from the webpage is sent to the class file(model), which filters it and sends the result back to flask, which in turn returns the result to the webpage as output.

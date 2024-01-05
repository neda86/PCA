# PCA implementation
You are provided with 2 synthetically generated json files, ’emails.json’ and ’emails new.json’. These can be imported and parsed with JuliaLang via
usingJSON; emails parsed = JSON.parsefile(”emails.json”);

- Import the 2 datasets and print the first email element of each parsed JSON, and also print how many unique words
exist in each string. (you may need to ’split’ the string into individual words).

- Produce a vector of all the unique words from all the emails which includes both files and also the length.

- Produce a function which will take in an email (string), and return a ’word vector’ of the normalized counts. This word vector is produced by making a dictionary with keys as all the possible words with values set to zero. Then for each word in the email seen the count of the word increments the value of the word key. Then normalize that vector.

- Produce a matrix for all the word vectors from the emails.json and then another matrix for the emails new.json. Each word vector comes from a single email string and the matrix will have these vectors appended to each other.
  
- Fit a PCA model to the data for the emails.json data and then visualize the values of the eigen values.

- Visualize the transfomed data from the 2 largest eigenvalue eigenvectors and project onto a scatter plot.

- Project the points of the emails new.json data onto the previous scatter plot and identify the email which is an outlier.

# Blaschko_BINF_final_project

For this project I studied what environmental factors contribute to antibiotic resistance in E. coli along with which machine learning models with which parameters work the best for large biological datasets. I used a large dataset from the UK Environmental Information Data Centre that sampled many different sources of E. coli in various areas of Bangladesh along with metadata about under what conditions the sample was taken. ([https://data.europa.eu/data/datasets/antibiotic-resistance-and-resistant-genes-in-escherichia-coli-from-human-poultry-and-en-2017-184?locale=en)](https://catalogue.ceh.ac.uk/documents/0239cdaf-deab-4151-8f68-715063eaea45)

I started with cleaning and preprocessing the data. I dropped out unnecessary columns. To deal with NA's, I subsetted the water samples because they had additional variables like pH, temp, and conductivity. I ran a random forest model on the subsetted water samples, created a feature importance graph, and did a grid search that iterated over different values of the max_depth and n_estimators parameters.

I plan to do the same analysis on the remaining samples of the dataset. I also plan to find the best-performing model among the random forest, a logistic regression, and a gradient boosting machine with different parameters to see which model handles this data the best. 

import pandas as pd

class SurveyAnalyzer:
    """
    A class to perform automatic statistical analysis on survey data.
    """

    def __init__(self, file_path):
        """
        Load the dataset from a CSV file.
        """
        self.df = pd.read_csv(file_path)

    def frequency(self, column):
        """
        Return the frequency count of a categorical column.
        """
        return self.df[column].value_counts()

    def crosstab(self, column1, column2):
        """
        Return a crosstab between two categorical variables.
        """
        return pd.crosstab(self.df[column1], self.df[column2])

    def mean_std(self, column):
        """
        Return the mean and standard deviation of a numerical column.
        """
        return {
            "mean": self.df[column].mean(),
            "std": self.df[column].std()
        }

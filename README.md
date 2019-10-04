﻿﻿﻿﻿﻿﻿﻿﻿﻿﻿﻿﻿﻿﻿﻿﻿﻿# **﻿3rd-ML100Days**The 3 round of the 100 days marathon on machine learning5. Day5: learn how to splice the sentence at every colume of a dataset by `` .splice()``8. Day8: ``hist()``10. Day10: learn how to use `.clip` to tricate the range of data. Hint: `.clip` contains the data on the broaderline.11. Day11: Here are two method to calculate mode in Python. One is the `from scipy.stats import mode`. The other is to count the most quantity number.13.  Day13: `cut()`  is to divide the data into several interval based on the bins, which exclud the lower bondary but includ the upper bondary.14.  Day14: using `corrcoef(x,y)` to analysis the correlation index of two array from `numpy` 15. Day15: using `pandas.corr()` to calculate the correlation index within a data frame16. Day16: using `seaborn.distplot()` or `seaborn.kdeplot()` to plot a Kernel Density Estimation17. Day17: using `pandas.cut()` to group the data by `bin =`, which is a list of boundaries within the data 18. Day 18: practice the `pandas.cutu()` and learn nothing new19. Day19: using `for i in range(len(x)):    matplotlib.pyplot(nrows, ncols, i+1)` to divide a graph into sub-graph based on their group20. Day20: `seaborn.heatmap()` create an easiest way to visualize the correlation between the columns of a data frame. You can set the gradient color, which is corresponded to the boundary `vmin = , vmax = ` by indicating `cmap = plt.cm.RdYlBu_r`,     The other way to create a heat map is using `seaborn.PairGrid()`. You could customize the matrix graph by using `.map_upper()`, `.map_diag()`, and `.map_lower()`. These correspond to the upper, diagonal, and lower part of a matrix. 22. Day22: Feature Engineering is to translate the text data into numerical format plus with a reasonable weight. The simplest feature engineering will need a `sklearn.preprocessing.LabelEncoder()` for transformation and a `sklearn.preprocessing.MinMaxScaler()` for normalization.23. Day23: Learn to normalized the data by `numpy.log1p()` and `stats.boxcox()`. The former is to translate the data into a natural log series. The later is to translate into different type of transformation based on the config of lambda. Be careful that `stats.boxcox()` requires the positive numerical series. It means every digits should be above 0.24. Day24: As described on Day 22, `sklearn.preprocessing.LabelEncoder()` could process the text-to-digits mapping but the amplitude of the digits means nothing. Another method is `pandas.get_dummies()`, a one-hot encoder automictically transform the category in one column into columns by the category. It eliminate the meaningless of quantity; however, it expand the structure of a data frame. The expansion may lower its efficiency of calculation.25. Day25: Unlike `pandas.get_dummies()`, mean coding is way to mitigate the structure expansion and equip with meaningful magnitude of the value, which is meaningless in `sklearn.preprocessing.LabelEncoder()` . The method, `.groupby([])[''].mean().reset_index()` , is to replace every column with the mean of the corresponded expected value.26. Day26: Compared to `sklearn.preprocessing.LabelEncoder()` , `pandas.get_dummies()`, and  `.groupby()[''].mean()`, it may fit moderately under the large quantity of unique number. Another method is `.map(lambda x: hash(x) % 10)` . A hash function calculate the input text into a specific number.27. Day27: Here are two methods to deal with date variables. One is `datetime.datetime.strptime()`, which can transform the string data into date form data. The other is `datetime.datetime.strftime()`, which extract the specified date variable from a column. 28. Day28: Geographical data may be considered with correction factor. longitude: latitude = cos(40.75):129. Day29: Corresponding to Day 25, here are several application with `.groupby([])['']`, i.e. mean, median, mode, max, and min.30. Day30: The way to diminish the dimension of feature is to filter, wrapper, and embedded the low correlated feature. The simplest way is `list(corr[(corr['Survived'] > 0.1) | (corr['Survived'] < -0.1)].index)`. The normalized way is `sklearn.linear_model.Lasso(alpha = 0.001)`.
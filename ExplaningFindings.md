# **OS Type vs Severity Level**
The 4 graphs shows the relation between“Severity Level” and“OS Type”. I manipulated the“OS Type” column to identify the specific types of“OS Type” associated with the network event was recorded. I used a histogram to visualise the trend. For all 4 graphs, the count is all relatively the same without much variation in the count for all 3“Severity Level”.

The histograms provided limited insight, so I conducted a chi-square test to further assess the relationship between“OS Type” and“Severity Level in more detail. The chi-square statistics were 16.11, which is a big value considering it has a degree of freedom of 6. This suggests that there is a strong association between the variables. Moreover, the p-value is 0.01, which is a lesser value compared to the threshold of 0.05. This means“OS Type” and“Severity Level” are associated. Lastly, I looked at the observed and expected frequency table which is shown below:

| OS Type | Low (Observed/Expected) | Medium (Observed/Expected) | High (Observed/Expected) |
| ------- | ----------------------- | -------------------------- | ------------------------ |
| Android | 503 / 533.10115         | 572 / 544.1275             | 545 / 541.1071           |
| Linux   | 2854 / 2913.443         | 2907 / 2969.135            | 3079 / 2957.422          |
| MacOS   | 3825 / 3818.885525      | 3868 / 3891.883625         | 3894 / 3876.43085        |
| Windows | 6001 / 5916.959975      | 6088 / 6029.1063875        | 5864 / 6006.17615        |

Based on the table, I can see that there is a large difference between the observed and expected frequency for all except MacOS, which further supports the previous findings of there being a strong relationship between“OS Type” and“Severity Level”. Thus, I conclude that there is a relationship between“OS Type” and“Severity Level”.

# **Timestamp vs Severity Level**
The graph explores the relationship between“Severity Level” and hours. I extracted the hour from the“Timestamp” column and highlighted business hours (9 AM to 5 PM) with a pink background. A line graph visualises the trend. The graph reveals no clear correlation between hours and“Severity Level,” as the lines are erratic without significant patterns

I also tried to find any relation between“Business Hours” and“Severity Level” by doing a Kruskal-Wallis H-Test. The results from the test were 2.31 for h-value which is relatively small and 0.32 for p-value which is significantly higher than the threshold of 0.05. Looking at both values suggests that the distributions of“Business Hours” differ across the categories of“Severity Level”. Thus, I conclude that there is no relationship between“Business Hours” and“Severity Level”.
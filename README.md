# Data-Mining-Final-Project

**LINK TO THE BOOK https://datamineaz.org/textbooks/hanDataMiningConceptual.pdf**

Big Topic: Heart Disease diagnoses and related correlation

sub topics:
1. food and heart disease
2. location and heart disease
   - Heart Disease by Location 2015-2017 (https://data.cdc.gov/Heart-Disease-Stroke-Prevention/Heart-Disease-Mortality-Data-Among-US-Adults-35-by/mfvi-hkb9)
   - Heart Disease by Location 2017-2019 (https://data.cdc.gov/Heart-Disease-Stroke-Prevention/Heart-Disease-Mortality-Data-Among-US-Adults-35-by/s6p7-fvbw)
   - Heart Disease by Location 2019-2021 (https://data.cdc.gov/Heart-Disease-Stroke-Prevention/Heart-Disease-Mortality-Data-Among-US-Adults-35-by/55yu-xksw)
4. other diseases and heart disease
5. life expectencies and heart disease

We each have by Sunday:
1. 2 good datasets or 1 amazingly huge one
2. clean preprocess data
3. start on clustering methods

Sunday: 
1. reevaluate goals
2. compare and contrast findings
3. optimize clustering

For Friday:
1. create data visualization

How to deal with Null data:

1.  Ignore the tuple: This is usually done when the class label is missing (assuming the mining task 
involves classification). This method is not very effective, unless the tuple contains several attributes 
with missing values. It is especially poor when the percentage of missing values per attribute varies 
considerably. By ignoring the tuple, we do not make use of the remaining attributes’ values in the 
tuple. Such data could have been useful to the task at hand.
2.  Fill in the missing value manually: In general, this approach is time consuming and may not be 
feasible given a large data set with many missing values. 
3.  Use a global constant to fill in the missing value: Replace all missing attribute values by the same 
constant such as a label like  “Unknown”  or −∞. If missing values are replaced by, say,  “Unknown,” 
then the mining program may mistakenly think that they form an interesting concept, since they all 
have a value in common—that of  “Unknown.”  Hence, although this method is simple, it is not 
foolproof. 
4. Use a measure of central tendency for the attribute (e.g., the mean or median) to fill in the miss-
ing value: Section 2.2 discussed measures of central tendency, which indicate the “middle” value 
of a data distribution. For normal (symmetric) data distributions, the mean can be used, whereas 
skewed data distribution should employ the median (Section 2.2). For example, suppose that the 
data distribution regarding the income of the customers is symmetric and that the mean income is 
$56,000. Use this value to replace the missing value for  income.
5.  Use the attribute mean or median for all samples belonging to the same class as the given 
tuple: For example, if classifying customers according to  credit_risk, we may replace the missing 
value with the mean  income  value for customers in the same credit risk category as that of the given 
tuple. If the data distribution for a given class is skewed, the median value is a better choice.
6.  Use the most probable value to fill in the missing value: This may be determined with regression, 
inference-based tools using a Bayesian formalism or decision tree induction. For example, using the 
other customer attributes in your data set, you may construct a decision tree to predict the missing 
values for  income. Decision trees, regression, and Bayesian inference are described in detail in 
Chapters 6 and 7.

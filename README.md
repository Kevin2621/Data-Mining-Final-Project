# Data-Mining-Final-Project

**LINK TO THE BOOK https://datamineaz.org/textbooks/hanDataMiningConceptual.pdf**

Big Topic: Heart Disease diagnoses and related correlation

sub topics:
1. food and heart disease
2. location and heart disease
   - Heart Disease by Location 2012-2014 (https://data.cdc.gov/Heart-Disease-Stroke-Prevention/Heart-Disease-Mortality-Data-Among-US-Adults-35-by/r35g-znws)
   - Heart Disease by Location 2015-2017 (https://data.cdc.gov/Heart-Disease-Stroke-Prevention/Heart-Disease-Mortality-Data-Among-US-Adults-35-by/mfvi-hkb9)
   - Heart Disease by Location 2017-2019 (https://data.cdc.gov/Heart-Disease-Stroke-Prevention/Heart-Disease-Mortality-Data-Among-US-Adults-35-by/s6p7-fvbw)
   - Heart Disease by Location 2019-2021 (https://data.cdc.gov/Heart-Disease-Stroke-Prevention/Heart-Disease-Mortality-Data-Among-US-Adults-35-by/55yu-xksw)
   - US Census Data County Population by Characteristics 2020-2023 (https://www.census.gov/data/tables/time-series/demo/popest/2020s-counties-detail.html)
   - US Census Data County Population by Characteristics 2010-2019 (https://www.census.gov/data/datasets/time-series/demo/popest/2010s-counties-detail.html)
4. other diseases, lifestyle, and heart disease
   - https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-County-Data-20/swc5-untb/explore/query/SELECT%0A%20%20%60year%60%2C%0A%20%20%60stateabbr%60%2C%0A%20%20%60statedesc%60%2C%0A%20%20%60locationname%60%2C%0A%20%20%60datasource%60%2C%0A%20%20%60category%60%2C%0A%20%20%60measure%60%2C%0A%20%20%60data_value_unit%60%2C%0A%20%20%60data_value_type%60%2C%0A%20%20%60data_value%60%2C%0A%20%20%60data_value_footnote_symbol%60%2C%0A%20%20%60data_value_footnote%60%2C%0A%20%20%60low_confidence_limit%60%2C%0A%20%20%60high_confidence_limit%60%2C%0A%20%20%60totalpopulation%60%2C%0A%20%20%60totalpop18plus%60%2C%0A%20%20%60locationid%60%2C%0A%20%20%60categoryid%60%2C%0A%20%20%60measureid%60%2C%0A%20%20%60datavaluetypeid%60%2C%0A%20%20%60short_question_text%60%2C%0A%20%20%60geolocation%60%0AWHERE%20caseless_one_of%28%60measure%60%2C%20%22Coronary%20heart%20disease%20among%20adults%22%29/page/filter
   - diseases and lifestyle by location (can group together through location to add lifestyle with it)
   - https://catalog.data.gov/dataset/behavioral-risk-factor-surveillance-system-brfss-national-cardiovascular-disease-surveilla
   - Identifies connections of cardiovascular disease and smoking/abnormal cholestoral and other factors
     https://data.cdc.gov/Chronic-Disease-Indicators/U-S-Chronic-Disease-Indicators-CDI-2023-Release/g4ie-h725/explore/query/SELECT%0A%20%20%60yearstart%60%2C%0A%20%20%60yearend%60%2C%0A%20%20%60locationabbr%60%2C%0A%20%20%60locationdesc%60%2C%0A%20%20%60datasource%60%2C%0A%20%20%60topic%60%2C%0A%20%20%60question%60%2C%0A%20%20%60response%60%2C%0A%20%20%60datavalueunit%60%2C%0A%20%20%60datavaluetype%60%2C%0A%20%20%60datavalue%60%2C%0A%20%20%60datavaluealt%60%2C%0A%20%20%60datavaluefootnotesymbol%60%2C%0A%20%20%60datavaluefootnote%60%2C%0A%20%20%60lowconfidencelimit%60%2C%0A%20%20%60highconfidencelimit%60%2C%0A%20%20%60stratificationcategory1%60%2C%0A%20%20%60stratification1%60%2C%0A%20%20%60stratificationcategory2%60%2C%0A%20%20%60stratification2%60%2C%0A%20%20%60stratificationcategory3%60%2C%0A%20%20%60stratification3%60%2C%0A%20%20%60geolocation%60%2C%0A%20%20%60responseid%60%2C%0A%20%20%60locationid%60%2C%0A%20%20%60topicid%60%2C%0A%20%20%60questionid%60%2C%0A%20%20%60datavaluetypeid%60%2C%0A%20%20%60stratificationcategoryid1%60%2C%0A%20%20%60stratificationid1%60%2C%0A%20%20%60stratificationcategoryid2%60%2C%0A%20%20%60stratificationid2%60%2C%0A%20%20%60stratificationcategoryid3%60%2C%0A%20%20%60stratificationid3%60%0AWHERE%20caseless_one_of%28%60question%60%2C%20%22Alcohol%20use%20among%20youth%22%29/page/filter
     - various health/behavior topics wioth year and location that can be grouped with heart disease
6. life expectencies and heart disease

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

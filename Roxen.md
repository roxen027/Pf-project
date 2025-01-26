```python
import pandas as pd 
```


```python
df=pd.read_csv("mba.csv")
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Undergraduate Major</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Current Job Title</th>
      <th>Annual Salary (Before MBA)</th>
      <th>Has Management Experience</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>MBA Funding Source</th>
      <th>Desired Post-MBA Role</th>
      <th>Expected Post-MBA Salary</th>
      <th>Location Preference (Post-MBA)</th>
      <th>Reason for MBA</th>
      <th>Online vs. On-Campus MBA</th>
      <th>Decided to Pursue MBA?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>27</td>
      <td>Male</td>
      <td>Arts</td>
      <td>3.18</td>
      <td>8</td>
      <td>Entrepreneur</td>
      <td>90624</td>
      <td>No</td>
      <td>688</td>
      <td>185</td>
      <td>7.9</td>
      <td>7.6</td>
      <td>Loan</td>
      <td>Finance Manager</td>
      <td>156165</td>
      <td>International</td>
      <td>Entrepreneurship</td>
      <td>On-Campus</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>24</td>
      <td>Male</td>
      <td>Arts</td>
      <td>3.03</td>
      <td>4</td>
      <td>Analyst</td>
      <td>53576</td>
      <td>Yes</td>
      <td>791</td>
      <td>405</td>
      <td>3.8</td>
      <td>4.1</td>
      <td>Loan</td>
      <td>Startup Founder</td>
      <td>165612</td>
      <td>International</td>
      <td>Career Growth</td>
      <td>Online</td>
      <td>No</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>33</td>
      <td>Female</td>
      <td>Business</td>
      <td>3.66</td>
      <td>9</td>
      <td>Engineer</td>
      <td>79796</td>
      <td>No</td>
      <td>430</td>
      <td>107</td>
      <td>6.7</td>
      <td>5.5</td>
      <td>Scholarship</td>
      <td>Consultant</td>
      <td>122248</td>
      <td>Domestic</td>
      <td>Skill Enhancement</td>
      <td>Online</td>
      <td>No</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>31</td>
      <td>Male</td>
      <td>Engineering</td>
      <td>2.46</td>
      <td>1</td>
      <td>Manager</td>
      <td>105956</td>
      <td>No</td>
      <td>356</td>
      <td>257</td>
      <td>1.0</td>
      <td>5.3</td>
      <td>Loan</td>
      <td>Consultant</td>
      <td>123797</td>
      <td>International</td>
      <td>Entrepreneurship</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>28</td>
      <td>Female</td>
      <td>Business</td>
      <td>2.75</td>
      <td>9</td>
      <td>Entrepreneur</td>
      <td>96132</td>
      <td>No</td>
      <td>472</td>
      <td>338</td>
      <td>9.5</td>
      <td>4.9</td>
      <td>Loan</td>
      <td>Consultant</td>
      <td>197509</td>
      <td>Domestic</td>
      <td>Skill Enhancement</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>9995</th>
      <td>9996</td>
      <td>33</td>
      <td>Female</td>
      <td>Economics</td>
      <td>3.55</td>
      <td>5</td>
      <td>Analyst</td>
      <td>109172</td>
      <td>Yes</td>
      <td>524</td>
      <td>100</td>
      <td>9.2</td>
      <td>8.0</td>
      <td>Loan</td>
      <td>Startup Founder</td>
      <td>69000</td>
      <td>International</td>
      <td>Networking</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>9996</th>
      <td>9997</td>
      <td>30</td>
      <td>Female</td>
      <td>Business</td>
      <td>2.48</td>
      <td>5</td>
      <td>Manager</td>
      <td>82515</td>
      <td>Yes</td>
      <td>330</td>
      <td>362</td>
      <td>7.4</td>
      <td>8.5</td>
      <td>Scholarship</td>
      <td>Consultant</td>
      <td>131054</td>
      <td>Domestic</td>
      <td>Entrepreneurship</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
    <tr>
      <th>9997</th>
      <td>9998</td>
      <td>31</td>
      <td>Female</td>
      <td>Economics</td>
      <td>2.86</td>
      <td>8</td>
      <td>Manager</td>
      <td>34152</td>
      <td>Yes</td>
      <td>681</td>
      <td>308</td>
      <td>6.8</td>
      <td>8.8</td>
      <td>Loan</td>
      <td>Consultant</td>
      <td>100806</td>
      <td>Domestic</td>
      <td>Networking</td>
      <td>On-Campus</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>9998</th>
      <td>9999</td>
      <td>22</td>
      <td>Female</td>
      <td>Arts</td>
      <td>2.30</td>
      <td>1</td>
      <td>Engineer</td>
      <td>61897</td>
      <td>No</td>
      <td>481</td>
      <td>190</td>
      <td>5.7</td>
      <td>7.7</td>
      <td>Self-funded</td>
      <td>Marketing Director</td>
      <td>115872</td>
      <td>International</td>
      <td>Networking</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>9999</th>
      <td>10000</td>
      <td>22</td>
      <td>Male</td>
      <td>Arts</td>
      <td>2.86</td>
      <td>2</td>
      <td>Manager</td>
      <td>111499</td>
      <td>No</td>
      <td>710</td>
      <td>226</td>
      <td>8.0</td>
      <td>1.7</td>
      <td>Employer</td>
      <td>Marketing Director</td>
      <td>103245</td>
      <td>Domestic</td>
      <td>Career Growth</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
  </tbody>
</table>
<p>10000 rows × 20 columns</p>
</div>




```python
df.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 10000 entries, 0 to 9999
    Data columns (total 20 columns):
     #   Column                          Non-Null Count  Dtype  
    ---  ------                          --------------  -----  
     0   Person ID                       10000 non-null  int64  
     1   Age                             10000 non-null  int64  
     2   Gender                          10000 non-null  object 
     3   Undergraduate Major             10000 non-null  object 
     4   Undergraduate GPA               10000 non-null  float64
     5   Years of Work Experience        10000 non-null  int64  
     6   Current Job Title               10000 non-null  object 
     7   Annual Salary (Before MBA)      10000 non-null  int64  
     8   Has Management Experience       10000 non-null  object 
     9   GRE/GMAT Score                  10000 non-null  int64  
     10  Undergrad University Ranking    10000 non-null  int64  
     11  Entrepreneurial Interest        10000 non-null  float64
     12  Networking Importance           10000 non-null  float64
     13  MBA Funding Source              10000 non-null  object 
     14  Desired Post-MBA Role           10000 non-null  object 
     15  Expected Post-MBA Salary        10000 non-null  int64  
     16  Location Preference (Post-MBA)  10000 non-null  object 
     17  Reason for MBA                  10000 non-null  object 
     18  Online vs. On-Campus MBA        10000 non-null  object 
     19  Decided to Pursue MBA?          10000 non-null  object 
    dtypes: float64(3), int64(7), object(10)
    memory usage: 1.5+ MB



```python
df.describe()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Annual Salary (Before MBA)</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>Expected Post-MBA Salary</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>10000.00000</td>
      <td>10000.000000</td>
      <td>10000.000000</td>
      <td>10000.00000</td>
      <td>10000.000000</td>
      <td>10000.00000</td>
      <td>10000.00000</td>
      <td>10000.000000</td>
      <td>10000.000000</td>
      <td>10000.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>5000.50000</td>
      <td>27.494300</td>
      <td>2.991611</td>
      <td>4.53350</td>
      <td>75166.406400</td>
      <td>524.44690</td>
      <td>247.03620</td>
      <td>5.477830</td>
      <td>5.522170</td>
      <td>130321.228900</td>
    </tr>
    <tr>
      <th>std</th>
      <td>2886.89568</td>
      <td>4.031823</td>
      <td>0.573509</td>
      <td>2.86166</td>
      <td>25850.070599</td>
      <td>158.06376</td>
      <td>144.87624</td>
      <td>2.585864</td>
      <td>2.588422</td>
      <td>40598.421993</td>
    </tr>
    <tr>
      <th>min</th>
      <td>1.00000</td>
      <td>21.000000</td>
      <td>2.000000</td>
      <td>0.00000</td>
      <td>30013.000000</td>
      <td>250.00000</td>
      <td>1.00000</td>
      <td>1.000000</td>
      <td>1.000000</td>
      <td>60001.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>2500.75000</td>
      <td>24.000000</td>
      <td>2.490000</td>
      <td>2.00000</td>
      <td>52862.000000</td>
      <td>390.00000</td>
      <td>121.00000</td>
      <td>3.200000</td>
      <td>3.300000</td>
      <td>95320.500000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>5000.50000</td>
      <td>27.000000</td>
      <td>2.990000</td>
      <td>5.00000</td>
      <td>74829.500000</td>
      <td>524.00000</td>
      <td>243.00000</td>
      <td>5.500000</td>
      <td>5.500000</td>
      <td>130155.500000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>7500.25000</td>
      <td>31.000000</td>
      <td>3.480000</td>
      <td>7.00000</td>
      <td>97273.000000</td>
      <td>661.00000</td>
      <td>373.00000</td>
      <td>7.700000</td>
      <td>7.700000</td>
      <td>165757.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>10000.00000</td>
      <td>34.000000</td>
      <td>4.000000</td>
      <td>9.00000</td>
      <td>119966.000000</td>
      <td>799.00000</td>
      <td>499.00000</td>
      <td>10.000000</td>
      <td>10.000000</td>
      <td>199999.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.sample()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Undergraduate Major</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Current Job Title</th>
      <th>Annual Salary (Before MBA)</th>
      <th>Has Management Experience</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>MBA Funding Source</th>
      <th>Desired Post-MBA Role</th>
      <th>Expected Post-MBA Salary</th>
      <th>Location Preference (Post-MBA)</th>
      <th>Reason for MBA</th>
      <th>Online vs. On-Campus MBA</th>
      <th>Decided to Pursue MBA?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>8785</th>
      <td>8786</td>
      <td>33</td>
      <td>Male</td>
      <td>Business</td>
      <td>3.91</td>
      <td>5</td>
      <td>Entrepreneur</td>
      <td>38489</td>
      <td>Yes</td>
      <td>350</td>
      <td>298</td>
      <td>6.9</td>
      <td>5.2</td>
      <td>Scholarship</td>
      <td>Consultant</td>
      <td>66653</td>
      <td>Domestic</td>
      <td>Career Growth</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Undergraduate Major</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Current Job Title</th>
      <th>Annual Salary (Before MBA)</th>
      <th>Has Management Experience</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>MBA Funding Source</th>
      <th>Desired Post-MBA Role</th>
      <th>Expected Post-MBA Salary</th>
      <th>Location Preference (Post-MBA)</th>
      <th>Reason for MBA</th>
      <th>Online vs. On-Campus MBA</th>
      <th>Decided to Pursue MBA?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>27</td>
      <td>Male</td>
      <td>Arts</td>
      <td>3.18</td>
      <td>8</td>
      <td>Entrepreneur</td>
      <td>90624</td>
      <td>No</td>
      <td>688</td>
      <td>185</td>
      <td>7.9</td>
      <td>7.6</td>
      <td>Loan</td>
      <td>Finance Manager</td>
      <td>156165</td>
      <td>International</td>
      <td>Entrepreneurship</td>
      <td>On-Campus</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>24</td>
      <td>Male</td>
      <td>Arts</td>
      <td>3.03</td>
      <td>4</td>
      <td>Analyst</td>
      <td>53576</td>
      <td>Yes</td>
      <td>791</td>
      <td>405</td>
      <td>3.8</td>
      <td>4.1</td>
      <td>Loan</td>
      <td>Startup Founder</td>
      <td>165612</td>
      <td>International</td>
      <td>Career Growth</td>
      <td>Online</td>
      <td>No</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>33</td>
      <td>Female</td>
      <td>Business</td>
      <td>3.66</td>
      <td>9</td>
      <td>Engineer</td>
      <td>79796</td>
      <td>No</td>
      <td>430</td>
      <td>107</td>
      <td>6.7</td>
      <td>5.5</td>
      <td>Scholarship</td>
      <td>Consultant</td>
      <td>122248</td>
      <td>Domestic</td>
      <td>Skill Enhancement</td>
      <td>Online</td>
      <td>No</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>31</td>
      <td>Male</td>
      <td>Engineering</td>
      <td>2.46</td>
      <td>1</td>
      <td>Manager</td>
      <td>105956</td>
      <td>No</td>
      <td>356</td>
      <td>257</td>
      <td>1.0</td>
      <td>5.3</td>
      <td>Loan</td>
      <td>Consultant</td>
      <td>123797</td>
      <td>International</td>
      <td>Entrepreneurship</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>28</td>
      <td>Female</td>
      <td>Business</td>
      <td>2.75</td>
      <td>9</td>
      <td>Entrepreneur</td>
      <td>96132</td>
      <td>No</td>
      <td>472</td>
      <td>338</td>
      <td>9.5</td>
      <td>4.9</td>
      <td>Loan</td>
      <td>Consultant</td>
      <td>197509</td>
      <td>Domestic</td>
      <td>Skill Enhancement</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.tail()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Undergraduate Major</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Current Job Title</th>
      <th>Annual Salary (Before MBA)</th>
      <th>Has Management Experience</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>MBA Funding Source</th>
      <th>Desired Post-MBA Role</th>
      <th>Expected Post-MBA Salary</th>
      <th>Location Preference (Post-MBA)</th>
      <th>Reason for MBA</th>
      <th>Online vs. On-Campus MBA</th>
      <th>Decided to Pursue MBA?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>9995</th>
      <td>9996</td>
      <td>33</td>
      <td>Female</td>
      <td>Economics</td>
      <td>3.55</td>
      <td>5</td>
      <td>Analyst</td>
      <td>109172</td>
      <td>Yes</td>
      <td>524</td>
      <td>100</td>
      <td>9.2</td>
      <td>8.0</td>
      <td>Loan</td>
      <td>Startup Founder</td>
      <td>69000</td>
      <td>International</td>
      <td>Networking</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>9996</th>
      <td>9997</td>
      <td>30</td>
      <td>Female</td>
      <td>Business</td>
      <td>2.48</td>
      <td>5</td>
      <td>Manager</td>
      <td>82515</td>
      <td>Yes</td>
      <td>330</td>
      <td>362</td>
      <td>7.4</td>
      <td>8.5</td>
      <td>Scholarship</td>
      <td>Consultant</td>
      <td>131054</td>
      <td>Domestic</td>
      <td>Entrepreneurship</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
    <tr>
      <th>9997</th>
      <td>9998</td>
      <td>31</td>
      <td>Female</td>
      <td>Economics</td>
      <td>2.86</td>
      <td>8</td>
      <td>Manager</td>
      <td>34152</td>
      <td>Yes</td>
      <td>681</td>
      <td>308</td>
      <td>6.8</td>
      <td>8.8</td>
      <td>Loan</td>
      <td>Consultant</td>
      <td>100806</td>
      <td>Domestic</td>
      <td>Networking</td>
      <td>On-Campus</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>9998</th>
      <td>9999</td>
      <td>22</td>
      <td>Female</td>
      <td>Arts</td>
      <td>2.30</td>
      <td>1</td>
      <td>Engineer</td>
      <td>61897</td>
      <td>No</td>
      <td>481</td>
      <td>190</td>
      <td>5.7</td>
      <td>7.7</td>
      <td>Self-funded</td>
      <td>Marketing Director</td>
      <td>115872</td>
      <td>International</td>
      <td>Networking</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>9999</th>
      <td>10000</td>
      <td>22</td>
      <td>Male</td>
      <td>Arts</td>
      <td>2.86</td>
      <td>2</td>
      <td>Manager</td>
      <td>111499</td>
      <td>No</td>
      <td>710</td>
      <td>226</td>
      <td>8.0</td>
      <td>1.7</td>
      <td>Employer</td>
      <td>Marketing Director</td>
      <td>103245</td>
      <td>Domestic</td>
      <td>Career Growth</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.describe(include="all")
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Undergraduate Major</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Current Job Title</th>
      <th>Annual Salary (Before MBA)</th>
      <th>Has Management Experience</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>MBA Funding Source</th>
      <th>Desired Post-MBA Role</th>
      <th>Expected Post-MBA Salary</th>
      <th>Location Preference (Post-MBA)</th>
      <th>Reason for MBA</th>
      <th>Online vs. On-Campus MBA</th>
      <th>Decided to Pursue MBA?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>10000.00000</td>
      <td>10000.000000</td>
      <td>10000</td>
      <td>10000</td>
      <td>10000.000000</td>
      <td>10000.00000</td>
      <td>10000</td>
      <td>10000.000000</td>
      <td>10000</td>
      <td>10000.00000</td>
      <td>10000.00000</td>
      <td>10000.000000</td>
      <td>10000.000000</td>
      <td>10000</td>
      <td>10000</td>
      <td>10000.000000</td>
      <td>10000</td>
      <td>10000</td>
      <td>10000</td>
      <td>10000</td>
    </tr>
    <tr>
      <th>unique</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>3</td>
      <td>5</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>5</td>
      <td>NaN</td>
      <td>2</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>4</td>
      <td>5</td>
      <td>NaN</td>
      <td>2</td>
      <td>4</td>
      <td>2</td>
      <td>2</td>
    </tr>
    <tr>
      <th>top</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>Male</td>
      <td>Economics</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Entrepreneur</td>
      <td>NaN</td>
      <td>No</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Employer</td>
      <td>Executive</td>
      <td>NaN</td>
      <td>International</td>
      <td>Networking</td>
      <td>On-Campus</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>freq</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>5073</td>
      <td>2082</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2034</td>
      <td>NaN</td>
      <td>6009</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2538</td>
      <td>2041</td>
      <td>NaN</td>
      <td>5083</td>
      <td>2546</td>
      <td>5005</td>
      <td>5907</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>5000.50000</td>
      <td>27.494300</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.991611</td>
      <td>4.53350</td>
      <td>NaN</td>
      <td>75166.406400</td>
      <td>NaN</td>
      <td>524.44690</td>
      <td>247.03620</td>
      <td>5.477830</td>
      <td>5.522170</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>130321.228900</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>std</th>
      <td>2886.89568</td>
      <td>4.031823</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0.573509</td>
      <td>2.86166</td>
      <td>NaN</td>
      <td>25850.070599</td>
      <td>NaN</td>
      <td>158.06376</td>
      <td>144.87624</td>
      <td>2.585864</td>
      <td>2.588422</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>40598.421993</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>min</th>
      <td>1.00000</td>
      <td>21.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.000000</td>
      <td>0.00000</td>
      <td>NaN</td>
      <td>30013.000000</td>
      <td>NaN</td>
      <td>250.00000</td>
      <td>1.00000</td>
      <td>1.000000</td>
      <td>1.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>60001.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>2500.75000</td>
      <td>24.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.490000</td>
      <td>2.00000</td>
      <td>NaN</td>
      <td>52862.000000</td>
      <td>NaN</td>
      <td>390.00000</td>
      <td>121.00000</td>
      <td>3.200000</td>
      <td>3.300000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>95320.500000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>5000.50000</td>
      <td>27.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.990000</td>
      <td>5.00000</td>
      <td>NaN</td>
      <td>74829.500000</td>
      <td>NaN</td>
      <td>524.00000</td>
      <td>243.00000</td>
      <td>5.500000</td>
      <td>5.500000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>130155.500000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>7500.25000</td>
      <td>31.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>3.480000</td>
      <td>7.00000</td>
      <td>NaN</td>
      <td>97273.000000</td>
      <td>NaN</td>
      <td>661.00000</td>
      <td>373.00000</td>
      <td>7.700000</td>
      <td>7.700000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>165757.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>max</th>
      <td>10000.00000</td>
      <td>34.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>4.000000</td>
      <td>9.00000</td>
      <td>NaN</td>
      <td>119966.000000</td>
      <td>NaN</td>
      <td>799.00000</td>
      <td>499.00000</td>
      <td>10.000000</td>
      <td>10.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>199999.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
a = df['Age']
a
```




    0       27
    1       24
    2       33
    3       31
    4       28
            ..
    9995    33
    9996    30
    9997    31
    9998    22
    9999    22
    Name: Age, Length: 10000, dtype: int64




```python
b = df[["Age","Gender"]]
b
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>10000.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>27.494300</td>
    </tr>
    <tr>
      <th>std</th>
      <td>4.031823</td>
    </tr>
    <tr>
      <th>min</th>
      <td>21.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>24.000000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>27.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>31.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>34.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
df['Undergraduate Major']
```




    0              Arts
    1              Arts
    2          Business
    3       Engineering
    4          Business
               ...     
    9995      Economics
    9996       Business
    9997      Economics
    9998           Arts
    9999           Arts
    Name: Undergraduate Major, Length: 10000, dtype: object




```python
df['Undergraduate GPA'].mean()
```




    2.991611




```python
df['Undergraduate GPA'].mode()
```




    0    2.77
    Name: Undergraduate GPA, dtype: float64




```python
df['Undergraduate GPA'].median()
```




    2.99




```python
df['Undergraduate GPA'].count()
```




    10000




```python
df['Undergraduate Major'].value_counts().plot(kind="bar")
```

    Matplotlib is building the font cache; this may take a moment.





    <Axes: xlabel='Undergraduate Major'>




    
![png](output_15_2.png)
    



```python
df['Undergraduate Major'].value_counts().plot(kind="barh")
```




    <Axes: ylabel='Undergraduate Major'>




    
![png](output_16_1.png)
    



```python
df['Undergraduate Major'].value_counts().plot(kind="hist")
```




    <Axes: ylabel='Frequency'>




    
![png](output_17_1.png)
    



```python
df['Undergraduate Major'].value_counts().plot(kind="box")
```




    <Axes: >




    
![png](output_18_1.png)
    



```python
df['Undergraduate Major'].value_counts().plot(kind="kde")
```




    <Axes: ylabel='Density'>




    
![png](output_19_1.png)
    



```python
df[['Undergraduate Major',"Age"]].value_counts().plot(kind="density")
```




    <Axes: ylabel='Density'>




    
![png](output_20_1.png)
    



```python
df["Age"].value_counts().plot(kind="pie")
```




    <Axes: ylabel='count'>




    
![png](output_21_1.png)
    



```python
df[["Years of Work Experience","Age"]].value_counts().plot(kind="pie")
```




    <Axes: ylabel='count'>




    
![png](output_22_1.png)
    



```python
df.isnull()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Undergraduate Major</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Current Job Title</th>
      <th>Annual Salary (Before MBA)</th>
      <th>Has Management Experience</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>MBA Funding Source</th>
      <th>Desired Post-MBA Role</th>
      <th>Expected Post-MBA Salary</th>
      <th>Location Preference (Post-MBA)</th>
      <th>Reason for MBA</th>
      <th>Online vs. On-Campus MBA</th>
      <th>Decided to Pursue MBA?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
    <tr>
      <th>1</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
    <tr>
      <th>3</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
    <tr>
      <th>4</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>9995</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
    <tr>
      <th>9996</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
    <tr>
      <th>9997</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
    <tr>
      <th>9998</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
    <tr>
      <th>9999</th>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
    </tr>
  </tbody>
</table>
<p>10000 rows × 20 columns</p>
</div>




```python
df.isnull().sum()
```




    Person ID                         0
    Age                               0
    Gender                            0
    Undergraduate Major               0
    Undergraduate GPA                 0
    Years of Work Experience          0
    Current Job Title                 0
    Annual Salary (Before MBA)        0
    Has Management Experience         0
    GRE/GMAT Score                    0
    Undergrad University Ranking      0
    Entrepreneurial Interest          0
    Networking Importance             0
    MBA Funding Source                0
    Desired Post-MBA Role             0
    Expected Post-MBA Salary          0
    Location Preference (Post-MBA)    0
    Reason for MBA                    0
    Online vs. On-Campus MBA          0
    Decided to Pursue MBA?            0
    dtype: int64




```python
df['Age'].isnull()
```




    0       False
    1       False
    2       False
    3       False
    4       False
            ...  
    9995    False
    9996    False
    9997    False
    9998    False
    9999    False
    Name: Age, Length: 10000, dtype: bool




```python
df.loc[[2,577,87,15,76]]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Undergraduate Major</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Current Job Title</th>
      <th>Annual Salary (Before MBA)</th>
      <th>Has Management Experience</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>MBA Funding Source</th>
      <th>Desired Post-MBA Role</th>
      <th>Expected Post-MBA Salary</th>
      <th>Location Preference (Post-MBA)</th>
      <th>Reason for MBA</th>
      <th>Online vs. On-Campus MBA</th>
      <th>Decided to Pursue MBA?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>33</td>
      <td>Female</td>
      <td>Business</td>
      <td>3.66</td>
      <td>9</td>
      <td>Engineer</td>
      <td>79796</td>
      <td>No</td>
      <td>430</td>
      <td>107</td>
      <td>6.7</td>
      <td>5.5</td>
      <td>Scholarship</td>
      <td>Consultant</td>
      <td>122248</td>
      <td>Domestic</td>
      <td>Skill Enhancement</td>
      <td>Online</td>
      <td>No</td>
    </tr>
    <tr>
      <th>577</th>
      <td>578</td>
      <td>25</td>
      <td>Male</td>
      <td>Science</td>
      <td>2.40</td>
      <td>7</td>
      <td>Manager</td>
      <td>44833</td>
      <td>No</td>
      <td>789</td>
      <td>54</td>
      <td>8.5</td>
      <td>7.3</td>
      <td>Loan</td>
      <td>Executive</td>
      <td>146811</td>
      <td>Domestic</td>
      <td>Skill Enhancement</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
    <tr>
      <th>87</th>
      <td>88</td>
      <td>24</td>
      <td>Female</td>
      <td>Business</td>
      <td>3.02</td>
      <td>2</td>
      <td>Entrepreneur</td>
      <td>44591</td>
      <td>No</td>
      <td>299</td>
      <td>140</td>
      <td>3.3</td>
      <td>8.8</td>
      <td>Scholarship</td>
      <td>Marketing Director</td>
      <td>89201</td>
      <td>Domestic</td>
      <td>Networking</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>15</th>
      <td>16</td>
      <td>24</td>
      <td>Male</td>
      <td>Economics</td>
      <td>2.03</td>
      <td>5</td>
      <td>Analyst</td>
      <td>62979</td>
      <td>No</td>
      <td>748</td>
      <td>4</td>
      <td>8.8</td>
      <td>8.7</td>
      <td>Self-funded</td>
      <td>Marketing Director</td>
      <td>173363</td>
      <td>Domestic</td>
      <td>Networking</td>
      <td>On-Campus</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>76</th>
      <td>77</td>
      <td>34</td>
      <td>Female</td>
      <td>Arts</td>
      <td>2.82</td>
      <td>4</td>
      <td>Engineer</td>
      <td>77841</td>
      <td>No</td>
      <td>315</td>
      <td>31</td>
      <td>4.5</td>
      <td>7.6</td>
      <td>Self-funded</td>
      <td>Consultant</td>
      <td>65161</td>
      <td>International</td>
      <td>Career Growth</td>
      <td>Online</td>
      <td>No</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.iloc[[27,99]]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Undergraduate Major</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Current Job Title</th>
      <th>Annual Salary (Before MBA)</th>
      <th>Has Management Experience</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>MBA Funding Source</th>
      <th>Desired Post-MBA Role</th>
      <th>Expected Post-MBA Salary</th>
      <th>Location Preference (Post-MBA)</th>
      <th>Reason for MBA</th>
      <th>Online vs. On-Campus MBA</th>
      <th>Decided to Pursue MBA?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>27</th>
      <td>28</td>
      <td>32</td>
      <td>Male</td>
      <td>Arts</td>
      <td>3.96</td>
      <td>9</td>
      <td>Entrepreneur</td>
      <td>64723</td>
      <td>No</td>
      <td>614</td>
      <td>417</td>
      <td>6.8</td>
      <td>5.4</td>
      <td>Employer</td>
      <td>Marketing Director</td>
      <td>85873</td>
      <td>International</td>
      <td>Skill Enhancement</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>99</th>
      <td>100</td>
      <td>34</td>
      <td>Male</td>
      <td>Arts</td>
      <td>3.80</td>
      <td>7</td>
      <td>Analyst</td>
      <td>40887</td>
      <td>No</td>
      <td>284</td>
      <td>9</td>
      <td>5.6</td>
      <td>4.4</td>
      <td>Scholarship</td>
      <td>Finance Manager</td>
      <td>65290</td>
      <td>Domestic</td>
      <td>Career Growth</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.groupby("Age").describe()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead tr th {
        text-align: left;
    }

    .dataframe thead tr:last-of-type th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th></th>
      <th colspan="8" halign="left">Person ID</th>
      <th colspan="2" halign="left">Undergraduate GPA</th>
      <th>...</th>
      <th colspan="2" halign="left">Networking Importance</th>
      <th colspan="8" halign="left">Expected Post-MBA Salary</th>
    </tr>
    <tr>
      <th></th>
      <th>count</th>
      <th>mean</th>
      <th>std</th>
      <th>min</th>
      <th>25%</th>
      <th>50%</th>
      <th>75%</th>
      <th>max</th>
      <th>count</th>
      <th>mean</th>
      <th>...</th>
      <th>75%</th>
      <th>max</th>
      <th>count</th>
      <th>mean</th>
      <th>std</th>
      <th>min</th>
      <th>25%</th>
      <th>50%</th>
      <th>75%</th>
      <th>max</th>
    </tr>
    <tr>
      <th>Age</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>21</th>
      <td>734.0</td>
      <td>4832.081744</td>
      <td>2916.495137</td>
      <td>30.0</td>
      <td>2239.50</td>
      <td>4794.0</td>
      <td>7316.75</td>
      <td>9989.0</td>
      <td>734.0</td>
      <td>2.971294</td>
      <td>...</td>
      <td>7.90</td>
      <td>10.0</td>
      <td>734.0</td>
      <td>128828.930518</td>
      <td>40573.106344</td>
      <td>60062.0</td>
      <td>94755.25</td>
      <td>129046.0</td>
      <td>163876.25</td>
      <td>199748.0</td>
    </tr>
    <tr>
      <th>22</th>
      <td>696.0</td>
      <td>5086.468391</td>
      <td>2906.837146</td>
      <td>22.0</td>
      <td>2537.75</td>
      <td>4979.5</td>
      <td>7765.00</td>
      <td>10000.0</td>
      <td>696.0</td>
      <td>2.977543</td>
      <td>...</td>
      <td>7.60</td>
      <td>10.0</td>
      <td>696.0</td>
      <td>128399.100575</td>
      <td>39840.732507</td>
      <td>60072.0</td>
      <td>95392.00</td>
      <td>128118.0</td>
      <td>161372.25</td>
      <td>199849.0</td>
    </tr>
    <tr>
      <th>23</th>
      <td>715.0</td>
      <td>4866.751049</td>
      <td>2880.589321</td>
      <td>10.0</td>
      <td>2354.50</td>
      <td>4724.0</td>
      <td>7349.00</td>
      <td>9995.0</td>
      <td>715.0</td>
      <td>3.003776</td>
      <td>...</td>
      <td>7.80</td>
      <td>10.0</td>
      <td>715.0</td>
      <td>128947.678322</td>
      <td>40713.150044</td>
      <td>60009.0</td>
      <td>94929.50</td>
      <td>129742.0</td>
      <td>163537.50</td>
      <td>199817.0</td>
    </tr>
    <tr>
      <th>24</th>
      <td>704.0</td>
      <td>5050.214489</td>
      <td>2848.531566</td>
      <td>2.0</td>
      <td>2718.75</td>
      <td>5053.5</td>
      <td>7400.75</td>
      <td>9992.0</td>
      <td>704.0</td>
      <td>2.961832</td>
      <td>...</td>
      <td>7.70</td>
      <td>10.0</td>
      <td>704.0</td>
      <td>130019.157670</td>
      <td>41120.843076</td>
      <td>60093.0</td>
      <td>93865.50</td>
      <td>130170.0</td>
      <td>165408.50</td>
      <td>199999.0</td>
    </tr>
    <tr>
      <th>25</th>
      <td>709.0</td>
      <td>4875.071932</td>
      <td>2924.131305</td>
      <td>7.0</td>
      <td>2441.00</td>
      <td>4666.0</td>
      <td>7416.00</td>
      <td>9994.0</td>
      <td>709.0</td>
      <td>2.995740</td>
      <td>...</td>
      <td>7.80</td>
      <td>10.0</td>
      <td>709.0</td>
      <td>130536.511989</td>
      <td>39570.573457</td>
      <td>60001.0</td>
      <td>97924.00</td>
      <td>128686.0</td>
      <td>164667.00</td>
      <td>199961.0</td>
    </tr>
    <tr>
      <th>26</th>
      <td>745.0</td>
      <td>5139.237584</td>
      <td>2848.176613</td>
      <td>20.0</td>
      <td>2723.00</td>
      <td>5232.0</td>
      <td>7492.00</td>
      <td>9985.0</td>
      <td>745.0</td>
      <td>3.011973</td>
      <td>...</td>
      <td>7.70</td>
      <td>10.0</td>
      <td>745.0</td>
      <td>131126.065772</td>
      <td>41322.732885</td>
      <td>60165.0</td>
      <td>94375.00</td>
      <td>132789.0</td>
      <td>166532.00</td>
      <td>199947.0</td>
    </tr>
    <tr>
      <th>27</th>
      <td>719.0</td>
      <td>5158.378303</td>
      <td>2934.898924</td>
      <td>1.0</td>
      <td>2639.00</td>
      <td>5302.0</td>
      <td>7795.00</td>
      <td>9966.0</td>
      <td>719.0</td>
      <td>2.980834</td>
      <td>...</td>
      <td>7.55</td>
      <td>10.0</td>
      <td>719.0</td>
      <td>131691.396384</td>
      <td>40779.642635</td>
      <td>60136.0</td>
      <td>94833.00</td>
      <td>132761.0</td>
      <td>169531.00</td>
      <td>199715.0</td>
    </tr>
    <tr>
      <th>28</th>
      <td>709.0</td>
      <td>4918.792666</td>
      <td>2859.082876</td>
      <td>5.0</td>
      <td>2443.00</td>
      <td>4831.0</td>
      <td>7295.00</td>
      <td>9981.0</td>
      <td>709.0</td>
      <td>2.972017</td>
      <td>...</td>
      <td>7.60</td>
      <td>10.0</td>
      <td>709.0</td>
      <td>130980.840621</td>
      <td>41555.888930</td>
      <td>60178.0</td>
      <td>95526.00</td>
      <td>132256.0</td>
      <td>167683.00</td>
      <td>199868.0</td>
    </tr>
    <tr>
      <th>29</th>
      <td>689.0</td>
      <td>4945.518142</td>
      <td>2849.932272</td>
      <td>36.0</td>
      <td>2521.00</td>
      <td>4867.0</td>
      <td>7467.00</td>
      <td>9986.0</td>
      <td>689.0</td>
      <td>2.978911</td>
      <td>...</td>
      <td>7.80</td>
      <td>10.0</td>
      <td>689.0</td>
      <td>129910.747460</td>
      <td>39413.981434</td>
      <td>60005.0</td>
      <td>96362.00</td>
      <td>129109.0</td>
      <td>163682.00</td>
      <td>199486.0</td>
    </tr>
    <tr>
      <th>30</th>
      <td>733.0</td>
      <td>5147.856753</td>
      <td>2976.147107</td>
      <td>9.0</td>
      <td>2509.00</td>
      <td>5371.0</td>
      <td>7714.00</td>
      <td>9997.0</td>
      <td>733.0</td>
      <td>3.016276</td>
      <td>...</td>
      <td>7.70</td>
      <td>10.0</td>
      <td>733.0</td>
      <td>131830.874488</td>
      <td>40333.131896</td>
      <td>60021.0</td>
      <td>99418.00</td>
      <td>129493.0</td>
      <td>166297.00</td>
      <td>199998.0</td>
    </tr>
    <tr>
      <th>31</th>
      <td>676.0</td>
      <td>5147.207101</td>
      <td>2804.390502</td>
      <td>4.0</td>
      <td>2664.75</td>
      <td>5284.5</td>
      <td>7431.25</td>
      <td>9998.0</td>
      <td>676.0</td>
      <td>3.012840</td>
      <td>...</td>
      <td>8.10</td>
      <td>10.0</td>
      <td>676.0</td>
      <td>129051.733728</td>
      <td>40411.880779</td>
      <td>60165.0</td>
      <td>93836.00</td>
      <td>129487.5</td>
      <td>165408.75</td>
      <td>199940.0</td>
    </tr>
    <tr>
      <th>32</th>
      <td>735.0</td>
      <td>4838.431293</td>
      <td>2900.731098</td>
      <td>24.0</td>
      <td>2386.00</td>
      <td>4678.0</td>
      <td>7331.50</td>
      <td>9979.0</td>
      <td>735.0</td>
      <td>2.994231</td>
      <td>...</td>
      <td>7.60</td>
      <td>10.0</td>
      <td>735.0</td>
      <td>130148.363265</td>
      <td>41088.151419</td>
      <td>60081.0</td>
      <td>95866.50</td>
      <td>129640.0</td>
      <td>166851.00</td>
      <td>199447.0</td>
    </tr>
    <tr>
      <th>33</th>
      <td>755.0</td>
      <td>5127.649007</td>
      <td>2857.749178</td>
      <td>3.0</td>
      <td>2605.00</td>
      <td>5240.0</td>
      <td>7559.00</td>
      <td>9996.0</td>
      <td>755.0</td>
      <td>2.988371</td>
      <td>...</td>
      <td>7.75</td>
      <td>10.0</td>
      <td>755.0</td>
      <td>131185.731126</td>
      <td>42331.304285</td>
      <td>60390.0</td>
      <td>92809.00</td>
      <td>132814.0</td>
      <td>169035.50</td>
      <td>199963.0</td>
    </tr>
    <tr>
      <th>34</th>
      <td>681.0</td>
      <td>4865.728341</td>
      <td>2884.218828</td>
      <td>25.0</td>
      <td>2363.00</td>
      <td>4791.0</td>
      <td>7411.00</td>
      <td>9965.0</td>
      <td>681.0</td>
      <td>3.017093</td>
      <td>...</td>
      <td>7.80</td>
      <td>10.0</td>
      <td>681.0</td>
      <td>131689.258443</td>
      <td>39073.853193</td>
      <td>60801.0</td>
      <td>96527.00</td>
      <td>133370.0</td>
      <td>165961.00</td>
      <td>199899.0</td>
    </tr>
  </tbody>
</table>
<p>14 rows × 72 columns</p>
</div>




```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Person ID</th>
      <th>Age</th>
      <th>Gender</th>
      <th>Undergraduate Major</th>
      <th>Undergraduate GPA</th>
      <th>Years of Work Experience</th>
      <th>Current Job Title</th>
      <th>Annual Salary (Before MBA)</th>
      <th>Has Management Experience</th>
      <th>GRE/GMAT Score</th>
      <th>Undergrad University Ranking</th>
      <th>Entrepreneurial Interest</th>
      <th>Networking Importance</th>
      <th>MBA Funding Source</th>
      <th>Desired Post-MBA Role</th>
      <th>Expected Post-MBA Salary</th>
      <th>Location Preference (Post-MBA)</th>
      <th>Reason for MBA</th>
      <th>Online vs. On-Campus MBA</th>
      <th>Decided to Pursue MBA?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>27</td>
      <td>Male</td>
      <td>Arts</td>
      <td>3.18</td>
      <td>8</td>
      <td>Entrepreneur</td>
      <td>90624</td>
      <td>No</td>
      <td>688</td>
      <td>185</td>
      <td>7.9</td>
      <td>7.6</td>
      <td>Loan</td>
      <td>Finance Manager</td>
      <td>156165</td>
      <td>International</td>
      <td>Entrepreneurship</td>
      <td>On-Campus</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>24</td>
      <td>Male</td>
      <td>Arts</td>
      <td>3.03</td>
      <td>4</td>
      <td>Analyst</td>
      <td>53576</td>
      <td>Yes</td>
      <td>791</td>
      <td>405</td>
      <td>3.8</td>
      <td>4.1</td>
      <td>Loan</td>
      <td>Startup Founder</td>
      <td>165612</td>
      <td>International</td>
      <td>Career Growth</td>
      <td>Online</td>
      <td>No</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>33</td>
      <td>Female</td>
      <td>Business</td>
      <td>3.66</td>
      <td>9</td>
      <td>Engineer</td>
      <td>79796</td>
      <td>No</td>
      <td>430</td>
      <td>107</td>
      <td>6.7</td>
      <td>5.5</td>
      <td>Scholarship</td>
      <td>Consultant</td>
      <td>122248</td>
      <td>Domestic</td>
      <td>Skill Enhancement</td>
      <td>Online</td>
      <td>No</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>31</td>
      <td>Male</td>
      <td>Engineering</td>
      <td>2.46</td>
      <td>1</td>
      <td>Manager</td>
      <td>105956</td>
      <td>No</td>
      <td>356</td>
      <td>257</td>
      <td>1.0</td>
      <td>5.3</td>
      <td>Loan</td>
      <td>Consultant</td>
      <td>123797</td>
      <td>International</td>
      <td>Entrepreneurship</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>28</td>
      <td>Female</td>
      <td>Business</td>
      <td>2.75</td>
      <td>9</td>
      <td>Entrepreneur</td>
      <td>96132</td>
      <td>No</td>
      <td>472</td>
      <td>338</td>
      <td>9.5</td>
      <td>4.9</td>
      <td>Loan</td>
      <td>Consultant</td>
      <td>197509</td>
      <td>Domestic</td>
      <td>Skill Enhancement</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>9995</th>
      <td>9996</td>
      <td>33</td>
      <td>Female</td>
      <td>Economics</td>
      <td>3.55</td>
      <td>5</td>
      <td>Analyst</td>
      <td>109172</td>
      <td>Yes</td>
      <td>524</td>
      <td>100</td>
      <td>9.2</td>
      <td>8.0</td>
      <td>Loan</td>
      <td>Startup Founder</td>
      <td>69000</td>
      <td>International</td>
      <td>Networking</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>9996</th>
      <td>9997</td>
      <td>30</td>
      <td>Female</td>
      <td>Business</td>
      <td>2.48</td>
      <td>5</td>
      <td>Manager</td>
      <td>82515</td>
      <td>Yes</td>
      <td>330</td>
      <td>362</td>
      <td>7.4</td>
      <td>8.5</td>
      <td>Scholarship</td>
      <td>Consultant</td>
      <td>131054</td>
      <td>Domestic</td>
      <td>Entrepreneurship</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
    <tr>
      <th>9997</th>
      <td>9998</td>
      <td>31</td>
      <td>Female</td>
      <td>Economics</td>
      <td>2.86</td>
      <td>8</td>
      <td>Manager</td>
      <td>34152</td>
      <td>Yes</td>
      <td>681</td>
      <td>308</td>
      <td>6.8</td>
      <td>8.8</td>
      <td>Loan</td>
      <td>Consultant</td>
      <td>100806</td>
      <td>Domestic</td>
      <td>Networking</td>
      <td>On-Campus</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>9998</th>
      <td>9999</td>
      <td>22</td>
      <td>Female</td>
      <td>Arts</td>
      <td>2.30</td>
      <td>1</td>
      <td>Engineer</td>
      <td>61897</td>
      <td>No</td>
      <td>481</td>
      <td>190</td>
      <td>5.7</td>
      <td>7.7</td>
      <td>Self-funded</td>
      <td>Marketing Director</td>
      <td>115872</td>
      <td>International</td>
      <td>Networking</td>
      <td>Online</td>
      <td>Yes</td>
    </tr>
    <tr>
      <th>9999</th>
      <td>10000</td>
      <td>22</td>
      <td>Male</td>
      <td>Arts</td>
      <td>2.86</td>
      <td>2</td>
      <td>Manager</td>
      <td>111499</td>
      <td>No</td>
      <td>710</td>
      <td>226</td>
      <td>8.0</td>
      <td>1.7</td>
      <td>Employer</td>
      <td>Marketing Director</td>
      <td>103245</td>
      <td>Domestic</td>
      <td>Career Growth</td>
      <td>On-Campus</td>
      <td>No</td>
    </tr>
  </tbody>
</table>
<p>10000 rows × 20 columns</p>
</div>




```python

```

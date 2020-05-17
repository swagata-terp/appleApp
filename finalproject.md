
## Introduction
This tutorial will help introduce a couple data science concepts. We will first curate data, then we shall visualize said data and evenutally use it to make predictions. Curation consists of taking out data that we will not be taking advantage of blah blah blah

## Dataset curation
blah blah insert text aout setting shit up


```python
import csv
import pandas as pd
import numpy as np
df = pd.read_csv('AppleStore.csv')
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
      <th>Unnamed: 0</th>
      <th>id</th>
      <th>track_name</th>
      <th>size_bytes</th>
      <th>currency</th>
      <th>price</th>
      <th>rating_count_tot</th>
      <th>rating_count_ver</th>
      <th>user_rating</th>
      <th>user_rating_ver</th>
      <th>ver</th>
      <th>cont_rating</th>
      <th>prime_genre</th>
      <th>sup_devices.num</th>
      <th>ipadSc_urls.num</th>
      <th>lang.num</th>
      <th>vpp_lic</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>281656475</td>
      <td>PAC-MAN Premium</td>
      <td>100788224</td>
      <td>USD</td>
      <td>3.99</td>
      <td>21292</td>
      <td>26</td>
      <td>4.0</td>
      <td>4.5</td>
      <td>6.3.5</td>
      <td>4+</td>
      <td>Games</td>
      <td>38</td>
      <td>5</td>
      <td>10</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>281796108</td>
      <td>Evernote - stay organized</td>
      <td>158578688</td>
      <td>USD</td>
      <td>0.00</td>
      <td>161065</td>
      <td>26</td>
      <td>4.0</td>
      <td>3.5</td>
      <td>8.2.2</td>
      <td>4+</td>
      <td>Productivity</td>
      <td>37</td>
      <td>5</td>
      <td>23</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>281940292</td>
      <td>WeatherBug - Local Weather, Radar, Maps, Alerts</td>
      <td>100524032</td>
      <td>USD</td>
      <td>0.00</td>
      <td>188583</td>
      <td>2822</td>
      <td>3.5</td>
      <td>4.5</td>
      <td>5.0.0</td>
      <td>4+</td>
      <td>Weather</td>
      <td>37</td>
      <td>5</td>
      <td>3</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>282614216</td>
      <td>eBay: Best App to Buy, Sell, Save! Online Shop...</td>
      <td>128512000</td>
      <td>USD</td>
      <td>0.00</td>
      <td>262241</td>
      <td>649</td>
      <td>4.0</td>
      <td>4.5</td>
      <td>5.10.0</td>
      <td>12+</td>
      <td>Shopping</td>
      <td>37</td>
      <td>5</td>
      <td>9</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>282935706</td>
      <td>Bible</td>
      <td>92774400</td>
      <td>USD</td>
      <td>0.00</td>
      <td>985920</td>
      <td>5320</td>
      <td>4.5</td>
      <td>5.0</td>
      <td>7.5.1</td>
      <td>4+</td>
      <td>Reference</td>
      <td>37</td>
      <td>5</td>
      <td>45</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>



# we need to tidy our data frame

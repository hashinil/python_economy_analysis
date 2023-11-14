# :moneybag::chart_with_upwards_trend: Economic Data Analysis :chart_with_downwards_trend::moneybag:

<!-- 
Reff vedio : https://www.youtube.com/watch?v=R67XuYc9NQ4
Data Set : https://www.kaggle.com/code/robikscube/economic-analysis-with-pandas-youtube-tutorial/notebook
-->

---------------------------------------------------

##### Technology:
- Python
  * Fred API <!-- fred_key='40378ef4ec282efb723bf3ac977aa973' -->
  * Pandas
  * Numpy
  * Matplotlib
  * Plotly

##### Data Collection:
  * Use [FRED API](https://pypi.org/project/fredapi/) to download data. 
    fredapi is a Python API for the FRED data provided by the Federal Reserve Bank of St. Louis. fredapi provides a wrapper in python to the FRED web service
    [Read more](https://mortada.net/python-api-for-fred.html)

---------------------------------------------------

##### Steps followed :
1. Connect to FRED API
- Create FRED object using Api key

    ```python
    from fredapi import Fred
    
    fred_key='PLACE_YOUR_KEY'
    fred = Fred(api_key=fred_key)
    ```

2. Search for S&P data
    ```python
    snp_data = fred.search('S&P', order_by='popularity')
    ```
    
3. Pull Raw Data & Plot
    ```python
    sp500 =  fred.get_series(series_id = 'SP500')
    sp500.plot(figsize=(10,5), title='S&P 500', lw=2)
    ```   
    ![image](https://github.com/hashinil/python_economy_analysis/assets/33922245/a25ebc15-4489-4d3f-97a2-21d4b0ac819c)

4. Pull and Join Multiple Data Series
    ```python
    
    ```   
<details>

<summary>Tips for collapsed sections</summary>

### You can add a header

You can add text within a collapsed section. 

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```

</details>


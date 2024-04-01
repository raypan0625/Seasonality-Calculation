# Seasonality-Calculation
Calculation of Seasonality based on past sales, category, and period covered

## Description
   - **Category 1**: Indoor/Outdoor
   - **Category 3-2**: Specific category of a category 1 item. e.g. Desk, Bar Stool, Fireplace...

## Calculations  
The seasonality is calculated using the monthly weight of all past rolling 12 months with the same period and took the average of each month's weight.   
For example, say we are in Sep 2023 right now, the [forecast](https://github.com/raypan0625/Item-SKU-Forecast) will be utilizing sales from Sep 2022-Aug 2023, so we found six segments with sales record of the same period: Sep 2017-Aug 2018, Sep 2018-Aug 2019, Sep 2019-Aug 2020, Sep 2020-Aug 2021, Sep 2021-Aug 2022, and Sep 2022-Aug 2023.   
With each of these periods, we compute the monthly weight values. Then we calculate the average weight for each month across all six periods to get our seasonality.

Note: *Seasonality for special categories (Christmas, Bean Bag, Fireplace, and Fire Pit)are calculated separately and are taken out from the calculation above.*  
  
Sample Indoor Seasonality:  
![image](https://github.com/raypan0625/Seasonality-Calculation/assets/103529023/05b2fed3-5ad7-48fe-9b58-4a7de1030f96)

Sample Outdoor Seasonality:  
![image](https://github.com/raypan0625/Seasonality-Calculation/assets/103529023/b04e2dc4-d864-48ef-8c74-78eefb9fdfd2)
  
## Author

Yulin Pan raypan0625@gmail.com

## Version History

* 0.1
    * Initial Release

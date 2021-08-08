# Challenge6

## Summary

The following project visulizes the San Francisco housing market. In the project, I use visualization tools in python, specifically hvplot and plotly. In addition, I integrated the mapbox api. In order to run this project you will need the following packages
1. Pandas
2. Plotly
3. HVplot

To complete the analysis, three data frames are provided that includes information on the housing market as well as latitude and longitutde information to soon down on the analysis. 

### Conclusion

Our analysis finds that the trend of price per square foot does not increase at the same rate as rental prices. A good opportunity for investors would be to look for markets with steady/decreasing price per square foot and buy these homes, while rental prices continue to increase. This is  a good investment opportunity because we do not see rental prices decreases in the data set provided.

**Housing unit increases**

![](https://github.com/bademola/Challenge6/blob/main/Starter_Code/Images/zoomed-housing-units-by-year.png)

**Anza Vista can be a potential investment!**

![](https://github.com/bademola/Challenge6/blob/main/Starter_Code/Images/pricing-info-by-neighborhood.png)


**Running the code below will give you an interactive code block**

`map_plot = px.scatter_mapbox(
    all_neighborhoods_df,
    lat= 'Lat',
    lon= 'Lon',
    size= 'sale_price_sqr_foot',
    color= 'gross_rent',
    zoom=11,
    size_max = 25,
    hover_name = 'Neighborhood'
)`


### If all imports are properly ran, an image similar to the below will render

![](https://github.com/bademola/Challenge6/blob/main/Starter_Code/Images/mapbox-plot.png)

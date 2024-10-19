Group 10 _ Boston Housing Dataset
* Subject: Data Science
* Member of group :
Nguyễn Quang Anh ( 22080296)
Triệu Anh (22080299)
Nguyễn Tú Anh (22080346)
Nguyễn Khánh Duy (22080310)
Nguyễn Hải Đăng (22080307)
Lê Quý Quỳnh Chi ( 22080305)



  Introduce:
  
   The Boston Housing Dataset Boston Housing Dataset is a famous dataset in the field of machine learning, often used for research and development of regression models. This dataset contains information on 506 neighborhoods within Boston, including characteristics such as real estate value, number of rooms, crime rate, and proximity to factors such as schools and shopping malls. commerce.


MEDIAN HOUSE VALUE DISTRIBUTION

![](image/ảnh1.png)

Analyze:

* The width of the above data ranges from 5 to 50, This fluctuation spectrum is quite wide, which shows the diverse distribution of house prices in Boston

* Distribution peak: The most popular home prices are between 20 and 25 thousand USD.

* Right skew: The graph has a slight right skew, meaning there are a small number of areas with very high home prices, but the majority of home prices are below average.

* Outliers: There are some values ​​near 50 thousand USD

* There are many factors that impact on house prices in Boston, but we'll pick three that we think have the biggest impact: location, value of use and objective social factors.

* Regarding Location, We analyze house prices based on location near the Charles River

* Value of Use : Room per dwelling

* Objective Social Factors: Crime Rating



MEDIAN HOUSE PRICE

![](image/ảnh2.png)


* Relationship between location near the river and house price:

Houses near the river (river_proximity = 1) have a significantly higher average price than houses not near the river (river_proximity = 0). This reflects the value of owning a home near a river, which is often a more desirable location for its views and fresh ai

* Volatility range:

Homes not close to the river have a wider price range, with some outliers going outside the box. This may indicate that even though there are some houses that are not close to the river, they still have a high value, possibly due to other factors such as size or quality of the hous.-

Homes near rivers have higher average values ​​and less variation than homes not near rivers. This shows that a location near the river can ensure a more stable home va

* Outliers:

There are many outliers at the top of the houses that are not close to the river, which suggests that there are some exceptional houses that command higher prices than the rest in this group. These homes may have other features that compensate for not being close to the river (for example, large size, other good locations, or high-end ameni tieConclusionclude: Proximity to the river is an important factor affecting home prices, and homes near the river often command higher prices. However, house prices not near the river also have large dispersion and may depend on factors other than geographical location.



HOUSE PRICED BASED ON NUMBERS OF ROOMS

![](image/ảnh3.png)


Positive relationship:

The scatter plot shows that there is a positive relationship between the average number of rooms and the average house price. As the number of rooms increases, house prices also tend to increase. This makes sense because homes with more rooms tend to be larger in size and have a higher value.
Data cluster: The majority of houses have 5 to 7 rooms and house prices range from about 15 to 35 thousand USD. This shows that this is a common price for average-sizehouse-

Exceptions:

There are some notable exceptions where houses have less than 6 rooms but house prices are very high (up to 50k USD). This could be due to other factors such as prime location or special features he househe h

Conclusion: 

The larger the average number of rooms, the higher the average home price, reflecting the fact that larger homes are generally worth more. The dispersion of the data also shows that there are houses with few rooms but still high prices, which may be related to factors other than house size.



HOUSE PRICED BASED ON CRIME RATED

![](image/ảnh4.png)


* The inverse relationship is quite clear. When crime rates increase, average home prices tend to plummet. This makes sense because areas with high crime rates are often not attractive places to buy a home, leading to lower home prices.

* In the areas with crime levels of 20% or more have very low house prices (under 10 thousand USD)

* Exceptions where crime rates ar quite high ( around 10%) but house prices are stillrelatively high. These cases may be affected by other factors such as the value of the house, climate, et

Conclution Social security in the Boston area is quite good with crime rates falling mostly below51%. This is a positive sign because house prices are greatly affected by this factrc


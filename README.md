# 1- Main Description 
Statistical Analysis 'll be performed on (OHLCV)Open-high-low-close Volume, BTC Data across different Time Frames.
The Findings Will be the 1st step in preparing for inputing the Data into an ML Live predictoin pipeline. 

## 2- Data available 
    1- Day OHLCV Bitcoin data from 1/1/2013 to 5/16/2022
    2- Second Bitcoin data from /1/2013 to 5/16/2022 (organzied in milliseconds)
Features of Data :
    1- UTC zone 
    2- Millisecond UNIX time stamps

## 3- Statistical Analysis Parameters: 
    For each Dataset Find the Following: 
        1- Mean , standard deviation ,distribution, variance, , max , min of : 
            1.1 Highs, Lows, open , close , Volume 
            1.2 Differences :
                1.2.1 High - low 
                1.2.2 low - high 
                1.2.3 open - close
                1.2.4 close - open
                1.2.5 Spot - PERP , in BTC & GMT Markets. 
        2- Correlation between : 
            2.1 BTC and Dow , s&p500, nasdaq , russel 2000 
            2.2 BTC and GMT 
            2.3 BTC-PERP & GMT-PERP
## 4- Data organization : 
    -The columns OHLCV will be Bucketized by Day fo the week UTC zone 
    -The columns OHLCV will be analyzed across Day, hour , minute Time frames To Extract : 
        -(This is based on the concepts in Finance like Volatility, But finance terms 'll not be necessarily used as We 'll treat this project as a Data science challenge)

## 4- Column mixes (Feature Crosses) : 
    - Feature crosses will be made to improve model time/ prediction accuracy & this section 'll be updated as the project develops. 

    ----------------------------------------------------------------------------------------------------------------------
# Findings : 
    1- GMT-PERP (Hour)
        Per hours of week. Minute data from 4/4/22 0:00 UTC to 5/23/22 0:00 UTC 
         1.1 High 
            Max: 3
            Min: 21
         1.2 Low 
            1.2.1 MAX 5 ,  , 2.45874375
            1.2.2 MIN 0 ,  , 2.41
        Open : 
            Max : 6,
            Min : 21
        Close : 
            max :  
            min: 
        Volume: 
            Max  :16
            Min : 21 

            Difference(high - low) : 
                MAX 16
                MIN: 22 
            Difference : (open - close): 
                MAX: 16
                MIN: 18
    2- GMT-PERP(Day)
        1.1 High 
            Max: 2
            Min: 6
         1.2 Low 
            1.2.1 MAX 1
            1.2.2 MIN 0
        Open : 
            Max : 2
            Min : 4
        Close : 
            max : 1
            min : 3 
        Volume: 
            MAx :2 
            Min : 6

            Difference(high - low) : 
                MAX : 3
                MIN :  6
            Difference : (open - close): 
                MAX:  3
                MIN:  1
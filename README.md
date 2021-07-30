# TelemetrySensorData

This project is inspired by one of the kaggle dataset titled Enviromental Sensor Telemetry Data. In this case there are three identical breadboard sensor that
placed in three different environment condition. The data itself contains 405,184 data that consists of nine columns. The following columns are:

      1. ts (timestamp) ==> epoch
      2. device id ==> object
      3. CO (Carbon Monoxide) in ppm ==> float64
      4. humidity in percent ==> float64
      5. light ==> bool
      6. LPG (liquified Petroleum Gas) in ppm ==> float64
      7. motion ==> bool
      8. smoke in ppm ==> float64
      9. Temperature in Fahrenheit ==> float64
      
All data gained by sensor reading that connected with raspberry pi. They are placed in different location, so we can know the condition of environment with
raspberry pi address. There are the following address and the environment where they are placed:

    1. 00:0f:00:70:91:0a ==> (stable conditions, cooler and more humid) 
    2. 1c:bf:ce:15:ec:4d ==> (highly variable temperature and humidity) 
    3. b8:27:eb:bf:9d:51 ==> (stable conditions, warmer and dryer) 

From this data I try to predict environment condition where sensor placed with features from sensor reading. I use machine learning algorithm to tackle this problem.

Source : https://www.kaggle.com/garystafford/environmental-sensor-data-132k

BME680:
===========
![BME680](https://github.com/linux-downey/picture_repository/blob/master/BME680.png)
BME680 is an integrated environmental sensor developed specifically for mobile applications and wearables where size and low power consumption are key requirements.It also supports four kinds of numerical measurements of temperature, humidity, gas and air pressure.  

Usage:
==========
***Bme680 supports IIC and SPI communication protocols.***
If the user uses IIC protocol,The main functions are as follows，And the results of mesurements stored in struct of bme680.sensor_result_value .  
    Seeed_BME680 bme680(IIC_ADDR); //IIC_ADDR is address of IIC device
    bme680.init();
    bme680.read_sensor_data();

If user uses SPI protocol,The main functions are as follows，And the results of mesurements stored in struct of bme680.sensor_result_value .  
    Seeed_BME680 bme680();//if user uses default pins of UNO development board.
  //  Seeed_BME680 bme680(BME_CS, BME_MOSI, BME_MISO,  BME_SCK);//if user customizes pin of SPI hardware interface.
    bme680.init();
    bme680.read_sensor_data();

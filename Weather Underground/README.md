## <font color="red">IMPORTANT: [Weather Underground stopped providing free API keys](https://www.wunderground.com/weather/api/)</font>
An alternative could be https://openweathermap.org/

This extension connects to the Weather Underground API. See also the [fantastic explanation](http://ai2.appinventor.mit.edu/reference/other/xml.html) at the App Inventor homepage

## Properties
* String ApiKey
  * Gets/sets your API Key. Get one at https://www.wunderground.com/weather/api/
* String LanguageCode
  * Gets/sets/ the language code of your request, as specified in the [documentation](https://www.wunderground.com/weather/api/d/docs?d=language-support)
* boolean UseBestForecast
  * Sets/gets whether to use Wunderground Best Forecast
* boolean UsePWS
  * Sets/gets whether to include Personal Weather Station in the report
* boolean Use XML
  * Sets/gets whether to use xml output

JsonTextDecode and XMLTextDecode have been copied from the Web component

## Methods
* GetForecast (int daysAndNights, String location)
  * Requests a weather forecast for `daysAndNights` in the future for `location`
* GetTide (int amount, String location)
  * Requests tidal information for `location` 
* GetAstronomy (String location)
  * Requests astronomical information for `location` (e.g. sunrise and sunset times)
* GetSatellite (String location)
  * Requests satellite images for `location`
* GetWebcams
  * Requests webcam images for `location`

For detailed information consult the .aia

## Events
* GotResponse (String url, int responseCode, String responseType, String responseContent, String requestType)
  * Event indicating that the request has finished

---

Current version number is 2

Note: XML does not work currently

[Visit this topic](https://community.thunkable.com/t/finally-here-weather-underground-api-extension/10791) at [Thunkable](http:/thunkable.com) for updates.
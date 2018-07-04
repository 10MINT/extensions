This extension connects to the Wolfram Alpha API

## Properties
* String AppID
  * Gets/sets the AppID. Get one at https://products.wolframalpha.com/api/
* String BackgroundColor _(only Simple API)_
  *  Gets/sets the background color of the resulting image. Not all colors can be used
* int Fontsize _(only Simple API)_
  * Gets/sets the font size to be used
* String ForegroundColor _(only Simple API)_
  *  Gets/sets the foreground color of the resulting image. Not all colors can be used
* int Width _(only Simple API)_
  * Gets/sets the width of the resulting image
* String Layout _(only Simple API)_
   * Sets/gets the layout to be used
   * either `labelbar` or `divider`
* int TimeoutTime
  * Sets/gets the time before the connection is timed out
* String Units
  * Sets/gets the units to be used
  * either `metric` or `imperial`

## Methods
* void GetFull (String request)
  * Sends a request to the Wolfram|Alpha Full Results API
* void GetSimple (String request)
  * Sends a request to the Wolfram|Alpha Simple API
* void GetShort (String request)
  * Sends a request to the Wolfram|Alpha Short Answers API
* void GetSpoken (String request)
  * Sends a request to the Wolfram|Alpha Spoken Results API

## Events
* GotResponse(String url, int responseCode, String responseType, String responseContent, String apiType)
  * Event indicating that the request has finished

---

Current version number is 3

[Visit this topic](https://community.thunkable.com/t/extension-for-wolfram-alpha/5081) at [Thunkable](http:/thunkable.com) for updates.
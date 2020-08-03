# Essentials extension
This extension bundles useful methods for App Inventor.
The following packages are included:

* ColorUtils
* ListUtils
* MathUtils
* ScreenUtils
* TextUtils

## ColorUtils
* **ColorToRgb** (Integer color)
   * Converts an App Inventor color to hex RGB
* **ColorToRgba** (Integer color)
   * Converts an App Inventor color to hex RGBA
* **RgbaToColor** (String color)
   * Converts hex RGBA to an App Inventor color

## ListUtils
Methods with the FromCopy ending do not change the list itself, but instead return a copy of the changed list
* **GetFirst** (List list) 
   * Returns the first object in the list
* **Pop** (List list) 
   * Removes the first object in the list and returns it
* **GetLast** (List list)
   * Returns the last object in the list
* **DropFirst**(List list) 
   * Removes the first object in the list
* **DropLast**(List list) 
   * Removes the last object in the list
* **Drop**(List list, Integer n)
   * Removes the first n objects from the list
* **Take** (List list, Integer n)
   * Keeps only the first n objects in list
* **RemoveAll** (List list, any item) 
   * Removes the object from the list
* **RemoveFirst** (List list, any item) 
   * Removes the object from the list once
* **Repeat** (List list, Integer n)
   * Repeats the list n times
* **Sort** (List list)
   * Sorts the list
   * Numbers and Instants are sorted by their natural order, lexiographic order
   is used as a fallback if the list contains different data types
   * Using mixed list can lead to unexpected results, be aware of that
* **SortBy** (List list, List walkingPath)
   * Sorts a list of lists by a `walkingPath`
   * A `walkingPath` is similar to the [walking key path](http://ai2.appinventor.mit.edu/reference/blocks/dictionaries.html#list-by-walking-key-path) of App Inventor dictionaries and contains the directions to the element to sort by
     * If you specify [1] as `waklingPath`, the list will be sorted by the first element of each list item.
     * You can go deeper, e.g. [2,3] will sort by the third element of the second element of each list item
   * All sorting rules from the Sort function apply

## MathUtils
* **isEven** (Number number)
   * returns true if number is even, false otherwise
   * even numbers can be divided by two without remainders
* **isPrime** (Number number)
   * returns true if the number is a prime number, false otherwise
* **isWhole** (Number number)
   * returns true if the number is whole, false otherwise
* **isPositive** (Number number)
   * returns true if the number is greater than zero, false otherwise
* **Invert** (Number x)
   * returns 1/x
* The constants **π**, **e**, **c** (in m/s), **g** (in m/s^2)
* **map**ping numbers from a scale to another scale
* conversion of
   * degree Celsius **toFahrenheit**
   * degree Fahrenheit **toCelsius**
   * miles **toKilometers**
   * kilometers **toMiles**
   
## ScreenUtils
* **IsCompanion**
   * whether the app runs in companion mode
* **SdkLevel**
   * returns the SDK level
* **AskForPermissions**
   * Ask for all permissions
* **PermissionsGranted**
   * Event that fires when all permissions were granted
* **PathToAssets**
   * returns the path to the assets
* **PathToData**
   * returns the path to the data folder
* **PathToSdcard**
   * returns the path to the sd card
* **Uri** (String filename)
   * returns the uri of the file

## TextUtils
* **StartsWith** (String text, String prefix)
   * returns true if the text starts with `prefix`
* **EndsWith** (String text, String suffix)
   * returns true if the text ends with `suffix`
* **Parse** (String text, String start, String end)
   * returns the text between `start` and `end`
* **Matches** (String text, String regex)
   * returns true if the text matches the regular expression
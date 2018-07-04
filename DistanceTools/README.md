This extension can measure the distance between two coordinates between two points with various formulas
* pythagorean(double a, double b)
  * Calculates the hypotenuse of a and b according to the Pythagorean theorem

The following methods are for calculating the distances between two points on earth. The input format is decimal degrees, like the built-in Location component

* gcDistance(double lat1, double lng1, double lat2, double lng2)
  * Calculates the great-circle distance between two points on a sphere
* haversineFormula(double lat1, double lng1, double lat2, double lng2)
  * Calculates the distance between two points on earth. This method has a higher accuracy than the vincenty formula for shorter distances
* vincentyFormula(double lat1, double lng1, double lat2, double lng2)
  * Calculates the distance between two points on earth with an average accuracy of 50 m

---

Current version number is 3

[Visit this topic](https://community.thunkable.com/t/distance-tools-extension/7175) at [Thunkable](http:/thunkable.com) for updates.
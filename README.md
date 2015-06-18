# Yahoo-Weather-Fix
The link in the weather.forecast result is broken and does not take you to the proper city.  

This is a work-around until such time the link gets fixed.  

It requires two calls to the Yahoo API.  The first is to get the information regarding the place and, as input, needs 
the postal code and the two character country code (seperated by a space) to get the woeid, country name, region 
name and city name.  The second gets the weather forecast using the returned woeid.  A new link is built using the 
results of the two queries and the bad link in replaced in the .description HTML.

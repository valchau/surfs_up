# surfs_up Project

## Overview of Surfs Up Statistical Analysis
### I have an idea
I have visited Hawaii in my past (visiting Honolulu for my honeymoon), but more recently, while on vacation in Hawaii, I visited my brother, Colehour, who owns a coffee farm on the Big Island (aka Hawaii) at the foot of the volcano, Mauna Loa. [Beautiful Hawaii](https://github.com/valchau/surfs_up/blob/main/Hawaii.PNG)

This is actually true, and yes you can really order from him here:  https://www.kanalaniohana.farm/farm. I also discovered that many people there really love surfing. I personally can't do it because I am pretty clumsy and can't even learn to swim, but I love my brother and his coffee. Also, recently there has been a terrible blight on the coffee trees and he is not making money this past year. See this: https://www.hawaiicoffeeed.com/clr.html

So I am trying to create a plan that will let me visit him more often, but also help him and his wife, who now has cancer to transition into another type of business that is not so dependent on the weather and bugs.  I thought a lot and come up with an idea that might work for him when his coffee and cocoa trees are not producing: a Surf and Coffee shop selling surfboards, along with coffee, chocolate and homemake jams to locals, tourists, and of course, our family. 

From my brother's website, the jams are already well liked: See:  https://www.kanalaniohana.farm/new-products "Available tropical jams are: lulo, lilikoi, guava, jaboticaba, marmalade, tamarillo, and basil.  Try something from our selection of cacao products:  Hot Chocolate Mix, Cacao Tea Elixir (cacao, turmeric, galangal), roasted cacao nibs, cocoa powder, and cacao husk tea. Coming soon-small batch 70% chocolate bars! "  

### Asking for funding
I have very little savings, so for this idea to work, we will need some real investor backing to help us start. I have taken classes in creating business plans, but  needed some help, and after putting together a strong business plan, I contacted an investor who wants to remain secret, so we will call him W. Avy, who is famous for his love of surfing. My first meeting with him goes extremely well, but he has one concern, what about the weather? I personally love the weather in Hawaii, but not everyone is me!

The potential investor is extremely serious about this. He invested in a surf shop early in his career. However, he didn't ask for any weather analysis and that early venture was rained out of existence. W. Avy hears that I have been learning how to properly analyze data and asks if I can run some analytics on a weather data set he has on the island O'ahu. That is far from my brother's coffee farm on the Big Island, but he is willing to go there. However, to get this investor to fund our startup, we need to provide him with some statistical data about the weather conditions in O'ahu that will convince him that this will be a successful business venture. While the given data is old, it is a start toward answering this investor's question about the precipitation. 

## Results
### How I analyzed the data
In order to give answers to this investor, I was able to obtain some weather data for O'hua in a SQLite database. I used Python and Jupyter Notebooks to import the weather data, and provide the statistical analyses requested. 

To begin, I read in the weather data from the SQLite database provided, which had data for 12 months, and created a Python DataFrame (using pandas) for temperature and precipiation. This data showed that there were 9 weather stations collecting temperature and precipitation data for this time period. I looked at the number of weather stations that were actively collecting precipitation data and chose the one station that had the most observations recorded for my analysis; it was station USC00519281. 

I then focused on observations that were recorded in the months of **June** and **December**, to see if winter vs. summer precipiation was different or not. 
I fould the following: 

* The average temperature is in the 70's year 'round. (similar to San Diego.)
* Both June and December showed similar high, low and average temperatures; with Decemeber being only about 3 degrees cooler.
* Therefore, a business such as a Surf Shop would be busy with tourists all year.

Here is what June looked like: low was 64 degrees, high was 85 degrees and the average was about 75 degrees in Fahrenheit.
[June Temperature Data](https://github.com/valchau/surfs_up/blob/main/June_Temp_stats.PNG)

Here is what December looked like: low was 56, high was 83, average was about 71 degrees in Fahrenheit. Not much lower than June's temperatures.
[December Temperature Data](https://github.com/valchau/surfs_up/blob/main/Dec_Temp_stats.PNG)

## Summary
Stats for station USC00519281 show that annually, the average precipitation was 17.7% based on 2,021  observations. This tells us that throughout the year, Oahu was mostly sunny throughout the day and experienced low rainfall. 
[Annual Precipitation Aug 2016 to Aug 2017 ](https://github.com/valchau/surfs_up/blob/main/precip_by_month_stats.PNG)

### Annual results
I found that the lowest temperature during the 12 month period measured was 54 degrees Fahrenheit and the highest temperature was 85 degrees Fahrenheit, with an average temperature of about 71 degrees Fahrenheit.

### Summer vs. Winter results
Comparing the termperatatures and precipitation for both June and December, I found the following:
* In summer there was only 14% average precipitation
* In winter, the lowest temperature at 56 degrees is actually cold, while the lowest temperature for summer (June) at 64 degrees, isn't so cold. Very similar weather at the coldest to San Diego. 
* For both summer and winter, the high temperatures, 83 degrees vs. 85 degrees were very similar, and much lower as a high temperature, than here in San Diego where it can be 100 degrees on a few weeks during summer and early fall. 
* For precipitation, the winter had more with a maximum value of 6.42, while summer's maximum value is 4.42. So yes it will rain more in Winter.

[Summer: Temp and Precipitation June ](https://github.com/valchau/surfs_up/blob/main/June_temp_precip.PNG)

[Winter: Temp and Precipitation Decemeber ](https://github.com/valchau/surfs_up/blob/main/Dec_temp_precip.PNG)

Looking at the precipitation and the temperature data for the years given, 2016 - 2017, I suspect that investing in a **Surf Shop** could be a viable business venture based solely on the decent weather of O'ahu, Hawaii. I would suggest further analysis, since 2023 is a long way in the future from the given set of data and climate change affects everywhere on Earth.


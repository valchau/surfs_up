# surfs_up Project

## Overview of Surfs Up Statistical Analysis
### I have an idea
I have visited Hawaii in my past (visiting Honolulu for my honeymoon), but more recently, while on vacation in Hawaii, I visited my brother, Colehour, who owns a coffee farm on the Big Island (aka Hawaii) at the foot of the volcano, Mauna Loa. [Beautiful Hawaii](https://github.com/valchau/surfs_up/blob/main/Hawaii.PNG)

This is actually true, and yes you can really order from him here:  https://www.kanalaniohana.farm/farm. I also discovered that many people there really love surfing. I personally can't do it because I am pretty clumsy and can't even learn to swim, but I love my brother and his coffee. Also, recently there has been a terrible blight on the coffee trees and he is not making money this past year. See this: https://www.hawaiicoffeeed.com/clr.html

So I am trying to create a plan that will let me visit him more often, but also help him and his wife, who now has cancer to transition into another type of business that is not so dependent on the weather and bugs.  I thought a lot and come up with an idea that might work for him when his coffee and cocoa trees are not producing: a Surf and Coffee shop selling surfboards, along with coffee, chocolate and homemake jams to locals, tourists, and of course, our family. 

From my brother's website, the jams are already well liked: See:  https://www.kanalaniohana.farm/new-products "Available tropical jams are: lulo, lilikoi, guava, jaboticaba, marmalade, tamarillo, and basil.  Try something from our selection of cacao products:  Hot Chocolate Mix, Cacao Tea Elixir (cacao, turmeric, galangal), roasted cacao nibs, cocoa powder, and cacao husk tea. Coming soon-small batch 70% chocolate bars! "  

### Asking for funding
I have very little savings, so for this idea to work, we will need some real investor backing to help us start. I have taken classes in creating business plans, but  needed some help, and after putting together a strong business plan, I contacted an investor who wants to remain secret, so we will call him W. Avy, who is famous for his love of surfing. My first meeting with him goes extremely well, but he has one concern, what about the weather? I personally love the weather in Hawaii, but not everyone is me!

The potential investor is extremely serious about this. He invested in a surf shop early in his career. However, he didn't ask for any weather analysis and that early venture was rained out of existence. W. Avy hears that I have been learning how to properly analyze data and asks if I can run some analytics on a weather data set he has on the island O'ahu. That is far from my brother's coffee farm on the Big Island, but he is willing to go there. However, to get this investor to fund our startup, we need to provide him with some statistical data about the weather conditions in O'ahu that will convince him that this will be a successful business venture.

### How I analyzed the data
In order to give answers to this investor, I was able to obtain some weather data in a SQLite database. I used Python and Jupyter Notebooks to import the data, and provide the statistical analyses requested. 

My starting analysis, where I read in the weather data, and created a Python DataFrame (using pandas) for temperature and precipiation data for the final 12 months of the given data. This represents August 23, 2016 - August 23, 2017. Here is how I did it: [climate analysis](https://github.com/valchau/surfs_up/blob/main/climate_analysis.ipynb)  There were 9 weather stations that gathered the data I used. Using the station with the most observations measured, the lowest temperature during the 12 month period measured was 54 degrees Fahrenheit and the highest temperature was 85 degrees Fahrenheit, with an average temperature of 71 degrees Fahrenheit.


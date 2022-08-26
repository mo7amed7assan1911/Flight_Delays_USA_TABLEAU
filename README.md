# 2015 Flight Delays and Cancellations in USA - Data Analysis

> You can find the original data [here](https://www.kaggle.com/datasets/usdot/flight-delays).

> **You can visit the interactive visualization from [here](https://public.tableau.com/app/profile/mohamed.hassan6400/viz/2015FlightDelaysandCancellationsinUSA-DataAnalysis/TheStory).**

## Using _Python_ to clean and organizing the 3 csv files to make one big dataset for analysis.
> I `cleaned` many columns like:
> * `CANCELLATION_REASON`: As i converted the non readable values like A, B, C to be more readable values like "CANCELLATION_REASON", "Weather", "National Air System" and if there is no cancellation it will be "NO-CANCELLATION".
> * I Created a new column called `DATE` that compins data from three columns "YEAR", "MONTHE", "DAY"
> * `Time columns`: I handeled the delteted zeros in times as it comes with the form HHMM but the zeros in the left removed as it is csv file. Then i converted this to a datetime data type.

> I also `merged` files with each others to creat one big dataset.
> * I `merged` the airports csv file with the flights csv file to get the destination and origin values in th same row.
> * Finally I `merged` the airline csv file with the merged file above to get the actual name of the airline.


---

## Using _Tableau_to Analyse the dataset.


> I preferred to use **gradient blue** in most of my visualization as it is the color of the sky and it is compatible with the flights we talk about in this project.

## It is consists of 4 slides:
### Slide 1
![image](https://user-images.githubusercontent.com/55090589/186915831-93640008-6a9e-4e80-b7d8-0cfb7e424864.png)

> **It is a visualization that shows how often each city was chosen as a destination and we can see that the most 3 cities were chosen are:**
> 
> * **Chicago** by **18,899** times.
> * **Atlanta** by **17,833** times.
> * **Dallas-Fort Worth** by **12,331** times.

> Design Choices:
> * A **bar chart** is the best suited here, as I had to plot the number of times each city had been chosen over 2015 which involves a comparison among items.
> * I used **blue color** which is warm for the eyes and compatible with flight insights.

### Slide 2
![image](https://user-images.githubusercontent.com/55090589/186915868-df5d4f74-2650-4ff2-9d25-9afb96feabbf.png)

> **It is a visualization that shows how often each city was chosen as a destination and we can see that the most 3 cities were chosen are:**
> 
> * **CA** by **33,331** times.
> * **TX** by **32,612** times.

> Design Choices:
> * A map is the best suitable here as I had to plot the states with their number of times chosen to be a destination. So, I used maps as it is geographical data.
> * I used **sequential blue color**, the darker the color is, the bigger the number of times this state is chosen.

> **Notice: Hovering on each state will show you the entire cities on this state.**


### Slide 3
![image](https://user-images.githubusercontent.com/55090589/186915900-d94c8470-1a0d-44fb-ab62-182da98c86d2.png)

> **It is a dashboard showing information about the flights’ cancellation and consists of 3 worksheets:**
> 
> 1. **The cancellation rate for each day in every month You choose.**
>    * This shows the change in the cancellation rate for each day on the month you choose or in all months.
>    
>    * ***Design Choices:***
> 	   *  **Line chart** is the best suitable here as I had to plot the number of cancelations over the days in a specific month the user chose which involves a comparison between days.
> 	   
>  2. **Cancellation reasons.**
>     * Chart that shows the main reasons that cancellate the flights in each month user choose.
>     * **This shows for the months of winter. the Weather was the main reason for the cancellation.**
>     * For all months:
>       * **Weather** canceled **2,397 flights.**
>       * **Airline/Carrier** canceled **1,260 flights.**
>       * **National Air System** canceled **776 flights.**
> 	 * ***Design Choices:***
> 		  * **Bubble chart** is the best suitable here as I had to plot the relationship between the number of cancellations and each reason in a specific month the user chose. The bigger the size of the bubble, the bigger the number of cancellations based on it.
> 		  * I used **sequential blue color**, to the 3 bubbles that I see will be quiet for the reader’s eyes.
> 
>   1. **Cancellation rate for each state:**
>      * This shows that for all months of filtration, **VT** state has the highest cancellation rate of **4.61%** for each flight.

>  * **Notice: Hovering on each state will show you the entire cities in this state.**
>  *  **I added a monthly filter** that helps the reader to see the analysis of all the dashboard charts in a specific month or all over the year.

### Slide 4
![image](https://user-images.githubusercontent.com/55090589/186915949-a3457081-c1f9-4683-8553-3546127f0ed2.png)

> * **It is a motion graph that shows the change of rank for the main reason causing cancelations over the months.**
> * **I made a motion control on the right. The reader just starts it and motion will start.**
> * This shows that the weather takes the 1st rank in the month of winter.

> * ***Design Choices***
>   * **Line chart** is the best suitable here as I had to plot the relationship between 3 categories over the months. So, it is a time-series chart.
>   * I used **sequential blue color**, for the 3 categories that I see will be quiet for the reader’s eyes.

> * **Notice**: make sure you start the motion.


### Slide 5 
![image](https://user-images.githubusercontent.com/55090589/186915965-88f22dc6-e95e-497a-9dd8-4fbd26679aee.png)

> **It is a visualization showing the quality of airlines.**
> * Based on the Delay rate which is calculated from the rate of arrival delay and departure delay combined.
> * This shows the best 3 airports are:
>   * **Alaska Airlines Inc by 144.12%** delay rate for each flight.
>   * **Hawaiian Airlines Inc by 198.68%** delay rate for each flight.
>   * **Delta Airlines Inc by 802.85%** delay rate for each flight.
>  * And **the worst** airline was **Spirit Airlines Inc** with a **3246.99%** delay rate for each flight.

> * ***Design Choices:***
> 	* A **bar chart** is the best suited here, as I had to plot the delay rate for each airport which involves a comparison among items.
> 	* I used **blue color** which is warm for the eyes and compatible with flight insights.

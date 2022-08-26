# 2015 Flight Delays and Cancellations in USA - Data Analysis

> You can find the original data [here](https://www.kaggle.com/datasets/usdot/flight-delays).

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
> **You can visit the interactive story from [here](https://public.tableau.com/app/profile/mohamed.hassan6400/viz/2015FlightDelaysandCancellationsinUSA-DataAnalysis/Themostchosencitiesasadestination).**

> I preferred to use **gradient blue** in most of my visualization as it is the color of the sky and it is compatible with the flights we talk about in this project.


### It is consists of 4 slides:
### Slide 1
> It is a visualization that shows how often each city was chosen as a destination and we can see that the most 3 cities were chosen are:
> * Chicago by 18,899 times.
> * Atlanta by 17,833 times.
> * Dallas-Fort Worth by 12,331 times.


![image](https://user-images.githubusercontent.com/55090589/186673146-6018a5e1-a5d3-4839-baa9-96deca82cb29.png)

### Slide 2
> It is just a bigger view for the last slide .. as it shows how often each state was chosen as a destination and we can see that the most 2 states were chosen are:
> * CA by 33,331 times.
> * TX by 32,612 times.

> Notice: Hovering on each state will show you the entire cities on this state.


![image](https://user-images.githubusercontent.com/55090589/186673281-c3d2602f-4184-49a2-adbf-407b22d86d02.png)

### Slide 3
> It is a **dashboard** showin informations about the flights cancellation and consists of 3 worksheets:
> 1. Cancellation rate for each day in every month `You choose`.
>    * This shows the change in the cancellation rate for each day on the month you choose or in all months.
>  2. Cancellation reasons.
>     * Chart that shows the main reasons that cancellate the flights in each month `You choose`.
>     * **This shows for the months of winter .. the Weather was the main reason for cancellation.**
>     * For all months:
>       * **Weather** canceled **2,397 flights.**
>       * **Airline/Carrier** canceled **1,260 flights.**
>       * **National Air System** canceled **776 flights.**
>   3. Cancellation rate for each state:
>      * This shows that for all months `VT` state has cancellation rate **4.61% for each flight.**
>      * **Notice: Hovering on each state will show you the entire cities on this state.**


![image](https://user-images.githubusercontent.com/55090589/186673426-30ef6061-bed5-4b3d-8ac1-e21b4aeaf761.png)

### Slide 4 
> It is a visualization showing the quality of airlines.
> * Based on the Delay rate which is calculated from the rate of arrival delay and departure delay combined.
> * This shows the best 3 airports are:
>   * **Alaska Airlines Inc by 144.12%** delay rate for each flight.
>   * **Hawaiian Airlines Inc by 198.68%** delay rate for each flight.
>   * **Delta Airlines Inc by 802.85%** delay rate for each flight.
>  * And the worst airline was Spirit Airlines Inc with a 3246.99% delay rate for each flight.

![image](https://user-images.githubusercontent.com/55090589/186673558-a6bae193-db3b-488c-ba17-708e073de2aa.png)


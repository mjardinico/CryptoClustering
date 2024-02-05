##  Module 19 Challenge
* Project Name: Crypto Clustering
* Submitted by:  Michael Jardinico
* Date Submitted: Feb 3, 2024

### Project Overview
`Utilize your understanding of Python and unsupervised learning techniques to determine whether cryptocurrency values are influenced by changes in price over 24-hour and 7-day periods.`

### Working Files
1. `Crypto_Clustering.ipynb`
2. `/Resources/crypto_market_data.csv`
    
### Instructions
1. GitHub Repository Setup:
    - Create a GitHub repository called `CryptoClustering`.
    - Clone the repository to your local computer using Git.

2. File Organization: 
    - Download the starter files from [Starter_Code](https://github.com/mjardinico/CryptoClustering/tree/main/Resources/Starter_Code).
    - Create a directory called `Resources` and save the `crypto_market_data.csv` in it.
    - Use the [Crypto_Clustering.ipynb](https://github.com/mjardinico/CryptoClustering/blob/main/Crypto_Clustering.ipynb) as the main code.

3. Dependencies
    - import pandas
    - import hvplot.pandas
    - from sklearn.cluster import KMeans
    - from sklearn.decomposition import PCA
    - from sklearn.preprocessing import StandardScaler
   
4. Prepare the Data
    - Use the `StandardScaler()` from `scikit-learn` to normalize the data
    - Create a DataFrame with the scaled data and set the "coin-id" index as shown below
    ![Crypto DataFrame](https://github.com/mjardinico/CryptoClustering/blob/main/Resources/crypto_dataframe1.png)
    
    - Create an elbow curve to find the best value of k 
    

5. Mapping Data:
    - Create a Leaflet map instance in your JavaScript file, and set its initial view coordinates.
    - Loop through the GeoJSON data and extract latitude and longitude information from `feature.geometry.coordinates[1]` and `feature.geometry.coordinates[0]`.
    - Create circle markers on the map using Leaflet's `L.circleMarker` function. The radius of the circles can be determined based on the earthquake magnitude from `var magnitude = feature.properties.mag`.

6. Popups:
    - For each circle marker, create a popup that displays place information. You can use Leaflet's `bindPopup` method.
    - Implement mouseover and mouseout event functions to control when the popups appear and disappear.

7. Color Coding by Depth:
    - Create a function called `getColor(depth)` that assigns a color based on the depth of the earthquake. The depth information can be obtained from `var depth = feature.geometry.coordinates[2]`.
    - You can define a color scale or range based on preset values and use this function to assign colors to the circle markers.

8. Depth Legend:
    - Create a legend for the earthquake depths with their preset values.
    - This legend can be created as an HTML element, and you can style it as needed.
    - Add the legend to the map using Leaflet's `L.control()` or by directly appending it to the HTML document. In this code, it was added to the HTML using CSS. Refer to `/static/style.css`
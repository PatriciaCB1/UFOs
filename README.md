# UFOs

## Overview Of The Analysis 
Having created a webpage for UFO sightings and a dynamic table that work as intended, the aim is to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date filter, I have added table filters for the city, state, country, and shape to allow users to further drill down into the sightings.




## Resources
- Data Sources:  data.js array
- Software / Languages / Packages / Libraries:  VS Code Version: 1.43.2, JavaScript, HTML


## Results 

### To update the site and table the following steps were taken:
- Removed the list element that created the button
- Created four more list elements: city, state, country, and shape similar to the "Enter Date" list element. Ensured each element hasthe same "id" as the object properties in the data.js file
- In the app.js file, created an empty filters variable to keep track of all the elements that change when a search is entered. This variable will be used to store the property “id” and the value that was entered from user input
- Wrote code for two functions updateFilters() and filterTable()
- The updateFilters() function replaced the handleClick() function and updated the filters variable 
- The filterTable() function will filter the table data by the value that is entered for the "id" that has changed
- Modified the event listener so that it detects a "change" on each input element and calls the updateFilters() function
- Inside the function updateFilters(), wrote code to update the filters based on user input
- Created a variable that saves the element that was changed using d3.select
- Created a variable that saves the value of the changed element’s property
- Create a variable that saves the attribute of the changed element’s id
- Wrote an if-else statement that checks if a value was changed by the user. If a value was changed, ensured it would add the element’s id as the property and the value that was changed to the filters variable. If a value was not entered, then it clears the element id from the filters variable
- Inside the updateFilters() function, wrote code call the filterTable() function 
- In the filterTable() function, wrote code to filter the table based on the user input that is stored in the filters variable
- Created a variable for the filtered data that is equal to the data that builds the table. This variable will hold the updated table data based on the user input.
- Loop through the filters object and store the data that matches the filter values in the variable 
- Rebuild the table with the filtered data by passing the variable created previously


### Results

The new webpage can now be used to search and filter UFO sightings by date, city, state, and country

### Summary 
While the edits have improved the webpage, further work could be made to the webpage by adding predictive text so the filter fields would autopopulate once a user starts typing.  This would negate the need for users to type in the full city name correctly for example.  


## Webpage Images

### Unfiltered

### Filtered

![Image 1](https://github.com/PatriciaCB1/Bikesharing/blob/main/Images/Screen%20Shot%202021-04-11%20at%209.08.02%20PM.png)

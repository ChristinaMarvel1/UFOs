# UFOs
JavaScript, Bootstrap, and UFOs


#Deliverable 1: Filter UFO sightings on multiple criteria (80 points)
Deliverable 1 Instructions
Using JavaScript and HTML, you’ll modify the code in your index.html file to create more table filters. In addition to the date filter you created in this module, you’ll add filters for the city, state, country, and shape, as shown in the following 

Using JavaScript, you’ll replace the handleClick() function in your app.js file with a new function that saves the element, value, and id of the filter that was changed. Then, you’ll create a new function to loop through the dataset and keep only the results that match the search criteria. The webpage will be updated with the search criteria after pressing "Enter".

Follow the instructions below and the numbered comments in the starter code to complete Deliverable 1.

1. Download the ufo_starterCode.js, rename it app.js, and place it in the js folder of your UFOs GitHub repository. The starter code includes the code used to populate the table from this module.

2. In the index.html file, remove the list (<li></li>) element that creates the button.

3. Create four more list elements: city, state, country, and shape. These will be similar to the "Enter Date" list element. Each element should have the same "id" as the object properties in the data.js file.

4. In Step 1 of the app.js file, create an empty filters variable to keep track of all the elements that change when a search is entered. This variable will be used in Step 5 to store the property “id” and the value that was entered from user input.

5. Next, you will need to write code for two functions whose names we’ve provided in the starter code, updateFilters() and filterTable().
The updateFilters() function will replace your handleClick() function and update the filters variable you created in Step 1.
The filterTable() function will filter the table data by the value that is entered for the "id" that has changed.

6. For Step 2, located before the buildTable(tableData) function at the end of the starter code, modify the event listener from this module so that it detects a "change" on each input element and calls the updateFilters() function.

7. In Step 3, we’ve provided the function, updateFilters(). Inside this function, you’ll write code in Steps 4-5 to update the filters based on user input.

8. In Step 4a, create a variable that saves the element that was changed using d3.select(this).

9. In Step 4b, create a variable that saves the value of the changed element’s property.

10. In Step 4c, create a variable that saves the attribute of the changed element’s id.

11. In Step 5, write an if-else statement that checks if a value was changed by the user (variable from Step 4b). If a value was changed, add the element’s id (variable from Step 4c) as the property and the value that was changed to the filters variable you created in Step 1. If a value was not entered, then clear the element id from the filters variable.

12. In Step 6, inside the updateFilters() function, call the filterTable() function that will be used in Step 7.

13. In the filterTable() function in Step 7, write code to filter the table based on the user input that is stored in the filters variable.

14. In Step 8, create a variable for the filtered data that is equal to the data that builds the table. This variable will hold the updated table data based on the user input.

15. In Step 9, loop through the filters object and store the data that matches the filter values in the variable created in Step 8.

16. In Step 10, rebuild the table with the filtered data by passing the variable created in Step 8.


17. Deploy the web app on your GitHub pages.


## Deliverable 2: A written report on the UFO analysis (README.md) (20 points)
Initialize your repository with a README, and write your analysis of Deliverable 1.

Deliverable 2 Instructions
For your written analysis, be sure to use complete and coherent sentences. Your written analysis should contain three sections, which cover the following:

1. Overview of Project: Explain the purpose of this analysis.

2. Results: Describe to Dana how someone might use the new webpage by walking her through the process of using the search criteria. Use images of your webpage during the filtering process to support your explanation.

3. Summary: In a summary statement, describe one drawback of this new design and two recommendations for further development.

# UFOs
## Overview of Project
The purpose of this analysis is to create a webpage with an aesthetically appealing layout that contains a table of data about UFO sightings. We want to ensure that can our webpage can filter through data in the table by parameters input by the user and only display matches to the inputs from the user. Our code for this project was written in JavaScript and the code for the webpage was written in HTML. Our data has also been referenced from a JavaScript file.


## Results: 
#### Describe how someone might use the new webpage by walking her through the process of using the search criteria. Use images of your webpage during the filtering process to support your explanation.
The user interface of this webpage is fairly straight forward. Once you have navigated to the webpage, it should appear as shown in the image below on the home page. 

[https://github.com/mdbinger/UFOs/blob/main/static/css/images/home_page.png]

Navigate toward the bottom of the page to view the entire table. Near the top of the table of UFO data, on the left side of the page, you should see several filter options (shown below) which you can input information into in order to filter the table to show only values that match what you put in. 

[insert screenshot of filter options]

DISCLAIMER: Please note that there are specific formats required for entry, which are reflected in the example text in each filter box shown in the image above. For example, searching for "Fresno" will not return any results, as the code is looking for an exact match to our dataset, which has city, state, country, and shape names all in lowercase letters and states and countries are abbreviated. As a result, in order to get the results for Fresno, California in the United States, you would have to input, "fresno" in the city filter, "ca" in the State filter, and "us" in the country filter. You can see the results of the correct and an incorrect version of this search below. 

##### Incorrect Search
[insert image of fresno search good and bad]

##### Correct Search


## Summary 
#### In a summary statement, describe one drawback of this new design and two recommendations for further development.

The search functions developed on this webpage are very powerful, however, one critical drawback is what I mentioned above in my results section. Currently, our filters need strict formatting to work properly. Entries cannot have any capitalizations, must be spelled correctly, and some entries must be abbreviated properly. Although our example text displays options in the correct format, it is not unreasonable to expect some people to make mistakes and have no indication of what went wrong. Our table does not currently display any message when no data matches, so our users may incorrectly assume that there is no information for the parameters they input, but they may have simply input the parameters in an incorrect format. 

To mitigate this issue, I recommend two ideas for further development of this webpage:
    1) Create an "error" message when no data matches the parameters input that states something along the lines of, "No data matches input criteria, please check to make sure inputs are properly formatted according to the examples displayed."
    2) Consider refactoring the code to be slightly more lenient in what it matches (i.e. able to match items with capital letters). This is just my opinion, but it may be better to show all loose matches and let the users distinguish between which items they care about rather than showing no matches at all because the user input was not matches exactly. 




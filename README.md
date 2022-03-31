## Overview

The purpose of this project is to create a dynamic webpage to present UFO sightings. To this end, we style the HyperText Markup Language (HTML) file with CSS Bootstrap v.4 content delivery network (CDN). We also utilize JavaScript D3 library to filter and create a table within the HTML file and therefore webpage.

---

## Resources

Data source:
    data.js
    nasa.jpg

<!-- "pip show <software>" in command prompt to see pip install ver -->
<!-- pip show code from https://stackoverflow.com/questions/10214827/find-which-version-of-package-is-installed-with-pip -->
Software:
    Visual Studio Code (VSCode) 1.63.2

---

<!-- Results: Describe to Dana how someone might use the new webpage by walking her through the process of using the search criteria. Use images of your webpage during the filtering process to support your explanation. -->
## Results

The top of the webpage contains a Jumbotron header followed by an article title on the left and paragraphs on the right. The page ends with a filter on the left and a table of UFO sightings on the right. Without any input to the filter, the table displays all 111 sightings. Notice there are five categories within the filter, namely date, city, state, country, and shape. 

![webTop](https://user-images.githubusercontent.com/96349090/161052517-94103374-326d-4173-a637-3452d3e2e6ff.png)

![webBottom](https://user-images.githubusercontent.com/96349090/161052557-19b65994-3313-45a4-99c5-fa77889fca74.png)

Any input should be of the same form as that of the placeholder within each text box. Any deviation from the form will result in the filter not executing as desired. For instance, incorrectly filling out the date 01/10/2010 instead of 1/10/2010, or using uppercase for any of the other fields. Once an input is correctly filled, change to the filter is detected if we press enter on the keyboard or click anywhere on the webpage. The table is subsequently updated. An example of filtering the data can be seen below where the table returns three sightings within the state of Oregon.

![webBottomFiltered](https://user-images.githubusercontent.com/96349090/161052600-55597381-ab88-4612-ad2e-6fc0eb49bc18.png)

---

<!-- Summary: In a summary statement, describe one drawback of this new design and two recommendations for further development. -->
## Summary

One drawback of the webpage's current design is that input error may hinder the user from obtaining the desired sightings, especially for the criteria of shape where the possibilities are not necessarily intuitive.

As such, one recommendation for modification is to create a dropdown menu for each field of the filter. If the user has more than one criteria to filter, the dropdown option for each subsequent field chosen gets dynamically narrower so the resulting table displayed is always non-empty. This also resolves the issue of filtering for one or more criteria where no data is available.

Another recommendation may be to create a button for the filter so that the user can complete updating the table when the appropriate fields are filled out. The current filter is updated every time a change occurs to the page, including inputting a new search criteria. If the user forgets to make a change such as press enter, the last criteria filled out in the filter will not be executed. By adding a button at the bottom of the filter this issue will be eliminated.
